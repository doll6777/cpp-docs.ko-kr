---
title: '방법: 관리되지 않는 리소스를 바이트 배열로 로드'
ms.custom: get-started-article
ms.date: 11/04/2016
helpviewer_keywords:
- native resources, loading into Byte array
- unmanaged resources, loading into Byte array
- native resources
ms.assetid: cdada6cd-6d42-437a-a90f-44a0b18d6a93
ms.openlocfilehash: 425def1cd0557298985148d7bb9f74da489643e8
ms.sourcegitcommit: 573b36b52b0de7be5cae309d45b68ac7ecf9a6d8
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/10/2019
ms.locfileid: "79544960"
---
# <a name="how-to-load-unmanaged-resources-into-a-byte-array"></a>방법: 관리되지 않는 리소스를 바이트 배열로 로드

이 항목에서는 <xref:System.Byte> 배열에 관리 되지 않는 리소스를 로드 하는 여러 가지 방법에 대해 설명 합니다.

## <a name="example"></a>예제

관리 되지 않는 리소스의 크기를 알고 있으면 CLR 배열을 미리 할당 한 다음 CLR 배열의 배열 블록에 대 한 포인터를 사용 하 여 배열에 리소스를 로드할 수 있습니다.

```cpp
// load_unmanaged_resources_into_Byte_array.cpp
// compile with: /clr
using namespace System;
void unmanaged_func( unsigned char * p ) {
   for ( int i = 0; i < 10; i++ )
      p[ i ] = i;
}

public ref class A {
public:
   void func() {
      array<Byte> ^b = gcnew array<Byte>(10);
      pin_ptr<Byte> p =  &b[ 0 ];
      Byte * np = p;
      unmanaged_func( np );   // pass pointer to the block of CLR array.
      for ( int i = 0; i < 10; i++ )
         Console::Write( b[ i ] );
      Console::WriteLine();
   }
};

int main() {
   A^ g = gcnew A;
   g->func();
}
```

```Output
0123456789
```

## <a name="example"></a>예제

이 샘플에서는 관리 되지 않는 메모리 블록에서 관리 되는 배열로 데이터를 복사 하는 방법을 보여 줍니다.

```cpp
// load_unmanaged_resources_into_Byte_array_2.cpp
// compile with: /clr
using namespace System;
using namespace System::Runtime::InteropServices;

#include <string.h>
int main() {
   char buf[] = "Native String";
   int len = strlen(buf);
   array<Byte> ^byteArray = gcnew array<Byte>(len + 2);

   // convert any native pointer to IntPtr by doing C-Style cast
   Marshal::Copy( (IntPtr)buf, byteArray, 0, len );
}
```

## <a name="see-also"></a>참고 항목

[C++ Interop 사용(암시적 PInvoke)](../dotnet/using-cpp-interop-implicit-pinvoke.md)
