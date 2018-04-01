#include <stdio.h>
#include <wchar.h>
+wchar_t *my_wstrchr(wchar_t *ws, wchar_t wc)
+{
+
while (*ws) {
+
if (*ws == wc)
+
return ws;
+
++ws;
+ }
+ return NULL;
+}
+
size_t my_wstrlen(const wchar_t *s)
{
const wchar_t *p = s;
