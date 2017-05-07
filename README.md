# Bike-Share-Analysis
the following is the portion of the code where i am really stuck for a long time:
   
                    # convert duration units from seconds to minutes
                    ### Question 3a: Add a mathematical operation below   ###
                    ### to convert durations from seconds to minutes.     ###
                    
                    new_point['duration'] = datetime.datetime(float(row['Duration'])).minute_______
                    
                    # reformat datestrings into multiple columns
                    ### Question 3b: Fill in the blanks below to generate ###
                    ### the expected time values.                         ###
                    trip_date = datetime.strptime(row['Start Date'], '%m/%d/%Y %H:%M')
                    new_point['start_date']  = trip_date.strftime('%Y-%m-%d')
                    new_point['start_year']  = trip_date.strftime('%y')________
                    new_point['start_month'] = trip_date.strftime('%m')________
                    new_point['start_hour']  = trip_date.strftime('%H')_______
                    new_point['weekday']     = trip_date.strftime('%A')________
                    
