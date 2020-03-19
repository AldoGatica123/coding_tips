# Go

## Language Tips

__Concurrency Tips:__  
Don't close receiving channels.  
Do not share a resource by accessing it, but by passing it.  

__Go concurrency toolset:__  
go routines  
channels  
select  
sync package  

__Communication Sequential Processes CSP:__  
Each process is built for sequential execution.  
Data is communicated between processes via channels.  
Not shared state!  
Scale by adding more of the same. 