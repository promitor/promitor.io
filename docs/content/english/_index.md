---
####################### Banner #########################
banner:
  title : "Bringing Azure Monitor metrics <br> where you need them"
  image : "images/banner-art.svg"
  content : "Ever needed those Azure Monitor metrics outside of Azure? We are here to help."
  button:
    enable : false
    label : "Contact Us"
    link : "contact"

##################### Feature ##########################
feature:
  enable : true
  title : "Why Use Promitor?"
  feature_item:
    # feature item loop
    - name : "Metrics-as-Code"
      icon : "fas fa-code"
      content : "Easy to declare metrics to scrape via metrics-as-code"
      
    # feature item loop
    - name : "Resource Discovery"
      icon : "fas fa-object-group"
      content : "Automatically discover Azure resources at-scale to scrape metrics for in your Azure subscriptions"
      
    # feature item loop
    - name : "Multiple Metric Sinks"
      icon : "fas fa-cloud"
      content : "Automatically pushes metrics to systems such as Atlassian Statuspage, Prometheus and StatsD"
      
    # feature item loop
    - name : "Container & Kubernetes-Friendly"
      icon : "fas fa-user-clock"
      content : "Easily deployable via Docker and optimized for Kubernetes through Helm"
      
    # feature item loop
    - name : "Linux & Windows"
      icon : "fas fa-tachometer-alt"
      content : "Lorem ipsum dolor sit amet consectetur adipisicing elit quam nihil"
      
    # feature item loop
    - name : "Any Azure Cloud Support"
      icon : "fas fa-cloud"
      content : "Lorem ipsum dolor sit amet consectetur adipisicing elit quam nihil"
      
    # feature item loop
    - name : "Open-Source"
      icon : "fas fa-heart"
      content : "Lorem ipsum dolor sit amet consectetur adipisicing elit quam nihil"
      


######################### Service #####################
service:
  enable : true
  service_item:
    # service item loop
    - title : "Use your metrics anywhere"
      images:
      - "images/sinks/prometheus.png"
      - "images/sinks/statsd.png"
      - "images/sinks/atlassian-statuspage.png"
      content : "Bring your Azure Monitor metrics where you need them the most, without all the friction. Easily configure what metrics you need and send them to one or more of our metric sinks in minutes.<br/><br/>Not seeing what you need? [Let us know](https://github.com/tomkerkhove/promitor/issues/new)!"
      button:
        enable : true
        label : "Check it out"
        link : "https://promitor.io/configuration/v2.x/runtime/scraper#metric-sinks"
        
    # service item loop
    - title : "Trusted By Others"
      images:
      - "images/end-users/adobe.png"
      - "images/end-users/walmart-labs.png"
      - "images/end-users/resdiary.png"
      - "images/end-users/trynz.png"
      - "images/end-users/vsoft.png"
      content : "These companies are using Promitor successfully in production to bring their metrics where they need them."
        
################### Screenshot ########################
screenshot:
  enable : true
  title : "Experience the best <br> workflow with us"
  image : "images/screenshot.svg"

  

##################### Call to action #####################
# call_to_action:
#   enable : true
#   title : "Ready to get started?"
#   image : "images/cta.svg"
#   content : "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Consequat tristique eget amet, tempus eu at consecttur."
#   button:
#     enable : true
#     label : "Contact Us"
#     link : "contact"
---
