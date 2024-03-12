platform :ios, '14.3.0'

target 'ToDoList' do

  use_frameworks!

  # Pods for ToDoList
  pod 'RealmSwift'
  pod 'SwipeCellKit'
  pod 'ChameleonFramework/Swift', :git => 'https://github.com/wowansm/Chameleon.git', :branch => 'swift5'

  post_install do |installer|
      installer.generated_projects.each do |project|
          project.targets.each do |target|
              target.build_configurations.each do |config|
                  config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
              end
          end
      end
  end


  
end
