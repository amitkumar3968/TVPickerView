##TVPickerView

TV picker view with increment decrement operators. This view is easy to configure and allows user to pick a value from values provided by delegate.

##Installation using CocoaPods
    
    1. First update all Ruby gems: [sudo] gem update
    2. Install the CocoaPods gem: [sudo] gem install cocoapods
    3. Setup CocoaPods on your system: pod setup
    
For [using CocoaPods](http://nsscreencast.com/episodes/5-cocoapods) watch this screencast.
    
##Installation without CocoaPods
    1. Clone the TVPickerView to some directory on your machine.
    2. Add the TVPickerView.h and TVPickerView.m to your project and use the TVPickerView.
##Usage
#1. Using Interface builder:
    1. Add a view to .xib file
    2. Set the class to TVPickerView.
    3. Just sets the datasource and delegate property.
    4. Implement the TVPickerViewDelegate and TVPickerViewDatasource methods.

#2. Using Code:

    TVPickerView *programaticallyCreatedTvPickerView = [[TVPickerView alloc] initWithFrame:CGRectMake(67, 100, 186, 40)];
    [programaticallyCreatedTvPickerView setDatasource:...];
    [programaticallyCreatedTvPickerView setDelegate:...];

pod 'LibComponentLogging-pods'

