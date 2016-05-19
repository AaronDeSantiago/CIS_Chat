# Uncomment this line to define a global platform for your project
platform :ios, ‘8.0’
# Uncomment this line if you're using Swift
 use_frameworks!

target 'iChavoChat-v2' do
pod "xmpp-messenger-ios"
end

target 'iChavoChat-v2Tests' do

end

target 'iChavoChat-v2UITests' do

end

post_install do |installer|
    `rm -rf Pods/Headers/Private`
    `find Pods -regex 'Pods\/.*\.modulemap' -print0 | xargs -0 sed -i '' 's/private header.*//'`
end

