# DumbTest for C
Totally minimal testing framework for C (and C++) language. It was created because i couldn't find some easy to use C testing framework and writting this mini version just seemed easier.

## Usage
Include the header file into your project.
``` cpp
TEST(RandomTest) {
    ASSERT_W(2 > 1);
    ASSERT_EQ(3, 3);
    return EXIT_SUCCESS;
}
```
Example of simple test. Test functions must return int and return 0 on success. They need to be registered in main like this.

``` cpp
int main(void) {
    RUN_TEST(RandomTest());
}
```
