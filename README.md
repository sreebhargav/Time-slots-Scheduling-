AvailableSlots.java – 1-Hour Free Time

This program finds all 1-hour time slots in a day (0 to 24) when all teams are free. It goes through each team’s busy times and marks when they are unavailable. Then it checks each hour to see when no one is busy.

Time: O(N + R)    // N = total number of busy intervals across all team

Space: O(R)       // R = range of time (0 to 24 hours)

BestKHourSlot.java – Most Available Members in K Hours

This builds on the 1-hour slot idea. Instead of needing everyone to be free, it finds a K-hour period when the most team members are available. It adds up the number of available members at each hour and checks which K-hour stretch has the highest total.

 Time: O(N + R)        // N = total intervals, R = time range (24)
 Space: O(1)           //fixed-size arrays and output


 Note: The first solution uses a fixed array since the time range (0 to 24) is small and known. For larger or unknown time ranges, we can use a map to track only the hours when availability changes, avoiding large arrays(size will be too big).
 
