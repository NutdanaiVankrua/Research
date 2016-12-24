## Cocoapods
dependency manager for Swift and Objective-C Cocoa projects

### How to install Cocoapods through bundler
1. Check if your computer has ruby installed, by running the command 'ruby —version'
2. (Optional) If ruby is not installed, please install first
3. Open terminal and run 'gem install b'
4. In terminal, redirect into your project and run the following command 'bundle init'
5. There will be a Gemfile created, then specify your dependencies. (Read more @http://bundler.io/)</br>
	
	source 'https://rubygems.org'</br>
	gem 'cocoapods','0.39.0'</br>

6. Create '.bundle/config' inside your existing project. (mkdir, touch, nano)
7. Inside the '.bundle/config' file, edit the following</br>
	
	BUNDLE_PATH: vendor/bundle</br>
	BUNDLE_DISABLE_SHARED_GEMS: '1' //for this read more @http://stackoverflow.com/questions/8104370/what-does-it-mean-bundle-disable-shared-gems-1</br>

8. In terminal, inside your xCode project, run command 'bundle install'
9. To run the specific gem install inside bundle, use the following command 'bundle exec ...'

### How to use Cocoapods
1. Run cmd 'bundle exec pod --version' to check cocoapods installations. 
2. Run cmd 'bundle exec pod init'
3. Specify the following: </br>

# Uncomment this line to define a global platform for your project</br>
platform :ios, '8.0'</br>

# Uncomment this line if you're using Swift</br>
# use_frameworks!</br>

target 'TestingBundlerAndCocoapods' do</br>
	pod 'MMDrawerController', '~> 0.5.7'</br>
end</br>

target 'TestingBundlerAndCocoapodsTests' do</br>
</br>
end</br>

target 'TestingBundlerAndCocoapodsUITests' do</br>
</br>
end</br>

4. Run cmd 'bundle exec pod install'

### References
*Bundler website ~> http://bundler.io/<br/>
*Cocoapods website ~> https://cocoapods.org/app<br/>
*Installing Cocoapods with bundler ~> https://guides.cocoapods.org/using/a-gemfile.html<br/>
*How to use Podfile ~> https://guides.cocoapods.org/using/the-podfile.html

