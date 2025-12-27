# Available-instances-for-vessel-planning
This repository holds the instances and required general data to be used in vessel planning optimization problems in the logistics offshore context. 

The content of this repositiry accounts by four files in .json format:

  installations_id_type.json:
  
    The type of each installation id {installation_id: installation_type}
    
  diesel_deck_cargo_supply_duration.json: 
  
    Diesel rate from vessel to maritime installation {deisel_rate}
    
    Supply duration of one deck cargo order unit in hours per type of installation {supply_duration_per_order_per_installation_type:{installation_id}
    
  installations_distance.json:
  
    Matrix of distances from each installation and supply base to the others units {installation_id + supply base: {installation_id + supplt base}
    
  instance_data.json:
  
    Information of all 104 instances {instance_id} 
    
      Cluster id {cluster}
      
      Number of installations {number_installations}
      
      Installations id {installation_id}
      
      Maximum voyage duration {max_voyage_duration}
      
      Volume of diesel (m3) order per installation {diesel_orders:{installation_id}
      
      Units of deck cargo order with due dates in hours {deck_cargo_orders:{installation_id:[{order_id, due_date}]}}
      
      Start and end of each delivery service time window in hours {installation_id:{time_window_id:{start , end}}}
      
      
