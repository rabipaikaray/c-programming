#include <string.h>

int romanToInt(char * s){
    if (NULL == s)
    {
        printf("NULL string\n");
        return -1;
    }
    int len = strlen(s);
    if (len == 0)
    {
        printf("strlen is zero\n");
        return -1;
    }
    int ans = 0;

    for (int i = len - 1; i >= 0; --i)
    {
        if((s[i]=='V' &&  i>0) && s[i-1]=='I'){
            ans+=4;--i;}
        
        else if((s[i]=='X' && i>0 ) && s[i-1]=='I'){
            ans+=9;--i;}
        
        else if((s[i]=='L' && i>0) && s[i-1]=='X'){
            ans+=40;--i;}
        
        else if((s[i]=='C' && i>0) && s[i-1]=='X'){
            ans+=90;--i;}
        
        else if((s[i]=='D' && i>0) && s[i-1]=='C'){
            ans+=400;--i;}
        
        else if((s[i]=='M' && i>0) && s[i-1]=='C'){
            ans+=900; --i;}
        
        else if(s[i] == 'I')
            ans += 1;
        else if(s[i] == 'V')
            ans += 5;
        else if(s[i] == 'X')
            ans += 10;
        else if(s[i] == 'L')
            ans += 50;
        else if(s[i] == 'C')
            ans += 100;
        else if(s[i] == 'D')
            ans += 500;
        else if(s[i] == 'M')
            ans += 1000;
    }

    return ans;
}