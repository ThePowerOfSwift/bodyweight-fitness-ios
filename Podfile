# Uncomment the next line to define a global platform for your project
platform :ios, '9.0'

target 'Bodyweight Fitness' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for Bodyweight Fitness
  pod 'RealmSwift'
  pod 'SwiftyJSON'
  pod 'RxSwift',         '~> 3.0'
  pod 'RxCocoa',         '~> 3.0'
  pod 'JTAppleCalendar', '~> 7.0'
  pod 'Eureka',          '~> 4.0.1'
  pod 'Fabric'
  pod 'Crashlytics'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
  	if ['Eureka'].include? target.name
  		target.build_configurations.each do |config|
  			config.build_settings['SWIFT_VERSION'] = '4.0'
  		end
  	end
  end
end