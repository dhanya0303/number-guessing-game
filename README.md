#include &lt;stdio.h&gt;
#include &lt;stdlib.h&gt;
#include &lt;string.h&gt;
struct Contact {
char name[50];
char phone[15];
};
int main() {
struct Contact c;
int choice;
printf(&quot;1. Add Contact\n&quot;);
printf(&quot;2. View Contact\n&quot;);
printf(&quot;Enter choice: &quot;);
scanf(&quot;%d&quot;, &amp;choice);
if(choice == 1) {
printf(&quot;Enter Name: &quot;);

scanf(&quot;%s&quot;, c.name);
printf(&quot;Enter Phone: &quot;);
scanf(&quot;%s&quot;, c.phone);
printf(&quot;Contact Saved Successfully!\n&quot;);
}
else if(choice == 2) {
printf(&quot;Feature under development.\n&quot;);
}
else {
printf(&quot;Invalid Choice\n&quot;);
}
return 0;
}
