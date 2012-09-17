##TVPickerView

TV picker view with increment decrement operators. 

This View is a picker view which allows to pick a value from values provided by datasource.
Navigation among values is done via increment and decrement indicator on the side.
 
A picker object requires the cooperation of a delegate for showing value of anelement and a data source for providing 
the numbers of elements. 
The delegate must adopt the TVPickerViewDelegate protocol and implement the required methods. 
The data source must adopt the TVPickerViewDatasource protocol and 
implement the required methods to return the number of elements.

##Installation using CocoaPods

CocoaPods is distributed as a ruby gem, installing it is as easy as running the following commands in the terminal:

    $ [sudo] gem install cocoapods
    $ pod setup

Then, Create a textfile and name it Podfile in your XCode project directory.
Then, edit the Podfile and mention your dependencies.
    
    $ edit Podfile
    platform : ios
    pod 'TVPickerView',     '~> 1.0.0'
    
Now install the dependencies in your project :

    $ pod install
    
Make sure to always open the Xcode workspace instead of the project file when building your project.

    $ open App.xcworkspace
    
For more see, [using CocoaPods](http://nsscreencast.com/episodes/5-cocoapods) screencast.
    
##Installation without CocoaPods
    1. Clone the TVPickerView using: 
        git clone git@github.com:taviscaios/TVPickerView.git.
    2. Add the TVPickerView.h and TVPickerView.m to your project and use the TVPickerView.
##Usage
#1. Using Interface builder:
    1. Add a view to .xib file
    2. Set the class of the view to TVPickerView.
    3. Just sets the datasource and delegate property.
    4. Implement the TVPickerViewDelegate and TVPickerViewDatasource methods.

#2. Using Code:

    TVPickerView *programaticallyCreatedTvPickerView = [[TVPickerView alloc] initWithFrame:CGRectMake(67, 100, 186, 40)];
    [programaticallyCreatedTvPickerView setDatasource:...];
    [programaticallyCreatedTvPickerView setDelegate:...];
    [view addSubview:programaticallyCreatedTvPickerView ];

pod 'LibComponentLogging-pods'

