#include "prak_stats.h"
#include "log.h"


PrakStats::PrakStats()
{
	L2_hits=0;
	L2_access=0;
	Dram_access=0;
}
		
PrakStats::~PrakStats()
{
	PRAK_LOG("###----STATS DESTRUCTOR---_###");
	PRAK_LOG("NUM OF L2 ACCESS:%lld",L2_access);
	PRAK_LOG("NUM OF L2 Hits:%lld",L2_hits);
	PRAK_LOG("NUM OF Dram ACCESS:%lld",Dram_access);
}
void
PrakStats:: incrementL2(bool cache_hit)
{
	if(cache_hit)
	{
		L2_hits+=1;
	}
	L2_access+=1;
}

void
PrakStats:: incrementDram()
{
	Dram_access+=1;
}


