---
{"dg-publish":true,"permalink":"/snippets/elly/","dgHomeLink":true,"dgPassFrontmatter":false}
---

~Elly

// clang++ -o test test.cc && ./test
#include <cstdio>

class A { int _a; };
class B : public A { int _b; };
class C { int _c; };

class D : public A, public C { int _d; };

int main() {
	A *a = new D;
	B *b = static_cast<B*>(a);   // legal
	A *a2 = static_cast<A*>(b);  // legal

	printf("%p %p %p\n", a, b, a2);

	D *d = static_cast<D*>(a);
	C *c = static_cast<C*>(d);

	printf("%p %p\n", d, c);

	return 0;
}

Tags:
  snippets, ~