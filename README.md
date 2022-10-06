# Swift vs Objective C

1.  filename.swift vs filename.m and filename.h

2.  @main vs main.m 

3.  import frameworkname vs #import<frameworkname.h or filename.h>

4.  class classnameimade: classname    
                                      vs   
                                            
                                            in filename.h
                                            @interface classnameimade: classname
                                            @end
                                            
                                            in filename.m
                                            @implementation
                                            @end
                                              
                                              
5. override func viewDidLoad(){}         vs  -(void) viewDidload{}

6. super.viewDidLoad()          vs   [super.viewDidLoad];


7. var propertynameimade: propertyname    vs @property propertyname propertynameimade;


# Objective C

```
//preprocessor command, which tells a Objective-C compiler to include Foundation.h file before going to actual compilation.
#import <Foundation/Foundation.h>

@interface SampleClass:NSObject
- (void)sampleMethod;
@end

@implementation SampleClass

- (void)sampleMethod {
   // Function which causes the message "Hello, World!" to be displayed on the screen.
   NSLog(@"Hello, World! \n");
}

@end

int main() {
   /* my first program in Objective-C */
   SampleClass *sampleClass = [[SampleClass alloc]init];
   [sampleClass sampleMethod];
   return 0;
}

```


## Defining a Method
The general form of a method definition in Objective-C programming language is as follows 

```
+ : Class Method
- : Instance Method
- (return_type) method_name:( argumentType1 )argumentName1 
joiningArgument2:( argumentType2 )argumentName2 ... 
joiningArgumentn:( argumentTypen )argumentNamen {
   body of the function
}
```


### Example

```
/* function returning the max between two numbers */
- (int) max:(int) num1 secondNumber:(int) num2 {
   
   /* local variable declaration */
   int result;
 
   if (num1 > num2) {
      result = num1;
   } else {
      result = num2;
   }
 
   return result; 
}
```



## In Xcode

```
#import <UIKit/UIKit.h>
#import "AppDelegate.h"

int main(int argc, char * argv[]) {
    NSString * appDelegateClassName;
    // related in NSAutoreleasePool for memory management
    @autoreleasepool {
        // Setup code that might create autoreleased objects goes here.
        appDelegateClassName = NSStringFromClass([AppDelegate class]);
    }
    return UIApplicationMain(argc, argv, nil, appDelegateClassName);
}
```


## Type

Static Vs Dynamic

```
int x;         vs       id y; (similar with void *)
at Complie              at Run(Lazy Binding)
```


## Qualifier

```
long
short
const (Similar with let in swift language)
unsigned (No negative)
signed
```

## Operators

Obejective C vs Swift

```
x++ or ++x   vs   x += 1 
```

## While

Objective C vs Swift

```
do{                         repeat{
                                         
 
} while(condition);         } while(condition)
```


## Basic Function Style

```
C vs Objective C vs Swift

Return_Type: RT
Function_Name: FN
Function_Type: FT
Parameter_Name: PN
Parameter_Type: PT

C:

RT FN(PT PN){
 return Something;
}

ex)
Int double(int x){
   return (2*x); 
}

Objective C:

-(RT) FN:(PT)PN{
 return Something;
}
or
+(RT) FN:(PT)PN{
 return Something;
}

ex) instance method

-(int) double:(int)x{
   return (2*x);
}

+(int) double:(int)x{
   return (2*x);
}

Swift:

func FN(PN: PT) -> RT{
 Something
}

ex)

func double(x: Int) -> Int{
 return 2*x
}

```




## More Function Style

```

C:

int add(int x, int y){
  return (x+y);
}


Objective C:

// 'and' is parameter label you can make, it could be 'with', 'second', 'andSecond', 'secParameter' and so on. 
// It is up to you.
-(int) add:(int)x and:(int)y{
  return (x+y);
}


Swift:

func add(Int: x, Int: y) -> Int{
  return x+y
}

```


Ref) Format Specifiers
https://developer.apple.com/library/archive/documentation/Cocoa/Conceptual/Strings/Articles/formatSpecifiers.html


Ref) A breif history of Objective C by Robert C. Martin
https://www.youtube.com/watch?v=fBHZ-k2zNoo

Ref) Objective C Tutorial
https://www.tutorialspoint.com/objective_c/objective_c_program_structure.htm
