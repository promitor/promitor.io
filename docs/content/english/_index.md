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
  title : "How Does Promitor Help?"
  feature_item:
    # feature item loop
    - name : "Metrics-as-Code"
      icon : "fas fa-code"
      content : "Easy to declare metrics to scrape via metrics-as-code"

    # feature item loop
    - name : "Any Azure Services"
      icon : "fas fa-cogs"
      content : "Easy to scrape any Azure service through one of our convenient scrapers or our Generic scraper."

    # feature item loop
    - name : "Resource Discovery"
      icon : "fas fa-satellite"
      content : "Automatically discover Azure resources at-scale to scrape metrics for in your Azure subscriptions"

    # feature item loop
    - name : "Multiple Metric Sinks"
      icon : "fas fa-chart-area"
      content : "Automatically makes metrics available in systems such as Atlassian Statuspage, OpenTelemetry, Prometheus and StatsD"

    # feature item loop
    - name : "Easy to Deploy"
      icon : "fas fa-cubes"
      content : "Easily deploy agents as containers on any container platform, but optimized for Kubernetes"

    # feature item loop
    - name : "Any Azure Cloud"
      icon : "fas fa-cloud"
      content : "Scrape resources in any Azure cloud, including sovereign clouds<br/>*(US Gov, Germany, China)*"

    # feature item loop
    - name : "Open-Source"
      icon : "fas fa-heart"
      content : "Promitor is free and open-source with best-effort support"

    # feature item loop
    - name : "Linux & Windows"
      icon : "fab fa-linux"
      content : "Support for running Promitor agents on Linux or Windows"



######################### Service #####################
service:
  enable : true
  service_item:
    # service item loop
    - title : "Use your metrics anywhere"
      images:
      - "images/sinks/prometheus.png"
      - "images/sinks/opentelemetry.png"
      - "images/sinks/statsd.png"
      - "images/sinks/atlassian-statuspage.png"
      content : "Bring your Azure Monitor metrics where you need them the most, without all the friction. Easily configure what metrics you need and send them to one or more of our metric sinks in minutes.<br/><br/>Not seeing what you need? [Let us know](https://github.com/tomkerkhove/promitor/issues/new)!"
      button:
        enable : true
        label : "Check it out"
        link : "https://docs.promitor.io/configuration/v2.x/runtime/scraper#metric-sinks"

    # service item loop
    - title : "Trusted By Others"
      images:
      - "images/end-users/adfinis.png"
      - "images/end-users/adobe.png"
      - "images/end-users/albert-heijn.png"
      - "images/end-users/axon.png"
      - "images/end-users/bryte-blue.png"
      - "images/end-users/resdiary.png"
      - "images/end-users/the-trade-desk.png"
      - "images/end-users/trynz.png"
      - "images/end-users/vsoft.png"
      - "images/end-users/walmart-labs.png"
      content : "These companies are using Promitor successfully in production to bring their metrics where they need them.<br/><br/>*Learn more the usage of end-user logos on our [legal page](/legal)*."

    # service item loop
    - title : "Supported by Microsoft"
      images:
      - "images/microsoft.png"
      content : "We are proud to be supported by Microsoft!<br/><br/>They provide Azure credits through their [open-source program](https://opensource.microsoft.com/azure-credits) that allows us to automatically test and verify the quality of Promitor.<br/><br/>Thanks to this program, we can keep offering Promitor for free."

################### Screenshot ########################
# screenshot:
#   enable : true
#   title : "Experience the best <br> workflow with us"
#   image : "images/screenshot.svg"

##################### Call to action #####################
# call_to_action:
#   enable : true
#   title : "Ready to get started?"
#   image : "images/logo.svg"
#   content : "Do you want to give Promitor a try?"
#   button:
#     enable : true
#     label : "Get Started"
#     link : "get-started"
---
