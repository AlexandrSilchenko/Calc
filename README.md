//
//  ViewController.m
//  Calc
//
//  Created by Admin on 20.07.15.
//  Copyright © 2015 Admin. All rights reserved.
//

#import "ViewController.h"

@interface ViewController ()

@end

@implementation ViewController

- (void)viewDidLoad {
    [super viewDidLoad];
    n = 0;
}

- (void)didReceiveMemoryWarning {
    [super didReceiveMemoryWarning];
}

- (IBAction)Press:(UIButton*)sender{
    n = [sender tag];
    NSString *str = [NSString stringWithFormat:@"%g",n];
    [Display setText:str];
}

@end


//
//  ViewController.h
//  Calc
//
//  Created by Admin on 20.07.15.
//  Copyright © 2015 Admin. All rights reserved.
//

#import <UIKit/UIKit.h>

@interface ViewController : UIViewController
{
    IBOutlet UILabel *Display;
    double n;
}

- (IBAction)Press:(UIButton*)sender;

@end





