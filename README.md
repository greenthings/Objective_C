### Swift vs Objective C

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


### Objective C

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
- (return_type) method_name:( argumentType1 )argumentName1 
joiningArgument2:( argumentType2 )argumentName2 ... 
joiningArgumentn:( argumentTypen )argumentNamen {
   body of the function
}
```
- : Instance Method

# Example

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


Ref) A breif history of Objective C by Robert C. Martin
https://www.youtube.com/watch?v=fBHZ-k2zNoo

Ref) Objective C Tutorial
https://www.tutorialspoint.com/objective_c/objective_c_program_structure.htm
