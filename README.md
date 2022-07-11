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



Ref) A breif history of Objective C by Robert C. Martin
https://www.youtube.com/watch?v=fBHZ-k2zNoo

Ref) Objective C Tutorial
https://www.tutorialspoint.com/objective_c/objective_c_program_structure.htm
