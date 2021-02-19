### TMS
TMS system is a logistics and warehousing management SaaS platform. The platform allows trucking companies of all sizes to signup and manage their customers, shipments, fleet, drivers, invoices etc all from a single website.
* tms.freightapp.com - The core TMS project
  * Worked with designers and stake holders to design a massive and boring TMS data entry/dashboard platform
  * Created WebApp with a heavily customized, UX friendly data entry process
  * Created backend with all TMS logic
  * Created and managed MySQL schema
  * Created complex pricing system that allows user to create their own price chart
  * Created batch invoice process that would take orders and apply the pricing system to create invoices
  * Created an API backend to allow other trucking companies to interface with TMS
  * Created an downstream shipment status check to fetch shipment status from 3rd party carriers
  * Created an EDI mapping system that decoded 204, 210, 214 etc and inserted them into the system
  * Project uses HTML/JS/NODE/SOCKETIO/PHP/MYSQL
* Driver App - Receive pickup and delivery requests, capture signatures and documents, provide truck location updates
  * Created an app to get new pickup/delivery requests
  * Manage requests status, upload images directly from app to TMS
  * Provide realtime location of truck
  * Alert customer when driver is on-route
  * Integrated truck mileage monitoring device
  * Cordova
* High value shipment monitoring - A realtime shipment location monitoring tool for ops
  * Created a trip based GEOFENCING component that tracks the location of the truck on a predefined route, and throw alerts when truck stops or goes off the route
  * Created a realtime monitoring board to display all high value shipment and their location and status
  * Created a data ingestion component that allows trucking companies to feed data from GPS trackers
  * HTML/JS/NODE/SOCKETIO
* TMS OCR web service - Customizable Data extraction from PDF file
  * Created a scalable and customizable data extraction web service to read client shipment information
  * Created a form creator to allow users to customize forms to be scanned
  * Added export to allow data to be exported automatically to TMS, CSV or as a customized export to other api
  * OCR uses Google Vision Engine and Tesseract as backup. 
  * HTML/JS/NODE/SOCKETIO

### Shipby
Shipby is the consumer and b2b driver portal for the TMS project
* Shipby.com
  * Site was designed with UX in mind first, then built
  * Shipby.com has no backend, the idea was to utilize TMS' API calls so this can mimic as a trucking company
  * Project built on ReactJS, styled-components
* Shipby App
  * App was designed with UX in mind and matching to the design of the site to create cohesiveness in design
  * App has no backend as it works similarly like Shipby.com, fully using TMS API
  * Project was built on React Native
  
### Cyclelution
Cyclelution is a company in the business of E-waste recycling. The Cyclelution app was created to interface with a .net backend
* Designed and developed a mobile app to interface with an waste recycling web application.
* App uses SOCKETIO as a connection gateway to the Cyclelution API.
* Wrote a customized react native package to interface with the mobile zebra label printer. 
* Project was built on React Native

### bmmpr
bmmpr is a connected car alarm that connects to your car via the odbII port. I started working on bmmpr when the 1st version of the app was already created.
* Create an entire AWS VPC setup with a Staging and Prod env, env consists of VPC, Cognito, Route53, EC2, MariaDB, SNS, API, CloudFront, S3
* Created an Admin portal
  * Created components to manage users, devices, device histories and such
  * Created b2b components to allow device data exports
  * Project built on ReactJS
* Created the bmmpr App
  * Updated and maintained the app code base
  * Migrated from dynamo to amplify eventually moving to create own EC2 backend
  * Created ways to persist a ble connection and rapid reconnect
  * Created ble UART decoding and encodings, and added firmware update via UART
  * App created in React Native
* Created the bmmpr Backend
  * Migrated Dynamo to RDS MariaDB
  * Implemented amplify
  * Created a backend for the app and admin portal
  * Implemented s3, image thumbnail creation, firmware server
  * Created synchronization process using Hologram's API to update device sim status
  * Backend created in NodeJS/Express

### Looptify
Looptify is a social media and subscription service app
* Backend
  * Added robust user subscription and item purchase control component
  * Added a shipping component that would work with shipping service provider on sending merchandise
  * Added cronjobs to check on shipment updates
  * Added CRUD for user/items/subscriptions
  * Added video streaming service from AWS
  * Built on NodeJS Express MariaDB
* Admin portal
  * Created User/Item/Orders CRUD
  * Added influencer-admin user models to allow users to create and manage their own inventory and store
  * Built on ReactJS
* App
  * Created app to pull posts, comments, orders and live video streaming feeds from BE
  * Ability to broadcast live video streams
  * Built on React native

### Nibble
Nibble is a tinder clone that nibbles user
* Created an App that would fetch a list of users from BE and display them
* Created swiping component that would allow user to `nibble` other users
* Created backend that would fetch users from MySQL db
* Setup automated build and deploy process
* Project uses NodeJS/Express and React Native

### Humble
Humble is a app that allows user to place wagers on weekly NFL games using the humble coin (cryptocurrency)
* Humble App
  * Created an app that would pull data from backend to create a Fantasy Football style betting app
  * App created in React Native
* Humble Admin portal
  * Created a portal used to manage all aspects of Humble system
  * Created dashboards to show critical statistics, check and balances, revenues etc
  * Created components that would synchronize with sports games prediction and stats API
  * Portal created in ReactJS
* Humble Backend
  * Created RDS schema running on MariaDB
  * Created backend functions mostly CRUD
  * Created Payment verification process to check for payments via apple in-app and google wallet
  * Added check and balance security measures to ensure all books are balanced
  * Backend created using NodeJS Express

### KW
Keller Williams App is a mobile app that allows user to search and see properties for sale. App is intended to allow the user to be able to make offers and contact the agent as well as completing the documentation process of the purchase
* Created components based on design
* Integrated with backend GraphQL to fetch and persist search results and filters
* Improved map and map marker and map cluster rendering performance
* Improved screen transitions
* Support Web team on updating and improving the WebApp
* Debugged builds, collected bugs on sentry
* Project uses React Native/ReactJS/GraphQL

### Subaru Clarion HUD
Dashboard for a touchscreen head-unit 
* Head Unit uses SmartAccess WebKit which limited the amount of memory available to the dashboard
* Vanilla JS was used to create and populate the dashboard
* A widget factory was created that allows user to create and customize user own widgets
* Implement SmartAccess SDK to control car stereo and mapping functions
* Project uses WebKIT so vanilla JavaScript was used to conserve memory
