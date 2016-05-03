#include "simulator.h"
#include "log.h"
#include "lock.h"
#include "fixed_types.h"

class PrakStats
{
	private:
		UInt64 L2_hits;
		UInt64 L2_access;
		UInt64 Dram_access;
	public:
		PrakStats();
		~PrakStats();
		void incrementL2(bool cache_hit);
		void incrementDram();
};
