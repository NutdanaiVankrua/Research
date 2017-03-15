## Cocoapods
A dependency manager for Swift and Objective-C Cocoa projects

<br/>
## Installation
<br/>
1. Check if your computer has ruby installed, by running the command `ruby —version`<br/>
2. (Optional) If ruby is not installed, please install first<br/>
3. Open terminal and run `gem install bundler`<br/>
4. In terminal, redirect into your project and run the following command `bundle init`<br/>
5. There will be a Gemfile created, then specify your dependencies. [Read more](http://bundler.io/)<br/>
	
	```
	source 'https://rubygems.org'
	gem 'cocoapods','1.0.0'
	```

6. Create `.bundle/config` inside your existing project. (mkdir, touch, nano)
7. Inside the `.bundle/config` file, edit the following

	```
	BUNDLE_PATH: vendor/bundle
	BUNDLE_DISABLE_SHARED_GEMS: '1' //for this read more @http://stackoverflow.com/questions/8104370/what-does-it-mean-bundle-disable-shared-gems-1
	```

8. In terminal, inside your xCode project, run command `bundle install`
9. To run the specific gem install inside bundle, use the following command `bundle exec ...`

<br/>
## Usage
1. Run cmd `bundle exec pod --version` to check cocoapods installations. 
2. Run cmd `bundle exec pod init`
3. Specify the following

	```
	# Uncomment this line to define a global platform for your project
	platform :ios, '8.0'

	# Uncomment this line if you're using Swift
	# use_frameworks!

	target 'TestingBundlerAndCocoapods' do
		pod 'MMDrawerController', '~> 0.5.7'
	end

	target 'TestingBundlerAndCocoapodsTests' do

	end

	target 'TestingBundlerAndCocoapodsUITests' do

	end
	```

4. Run cmd `bundle exec pod install`

<br/>
## References
* [Bundler website](http://bundler.io/)
* [Cocoapods website](https://cocoapods.org/app)
* [Installing Cocoapods with bundler](https://guides.cocoapods.org/using/a-gemfile.html)
* [How to use Podfile](https://guides.cocoapods.org/using/the-podfile.html)

