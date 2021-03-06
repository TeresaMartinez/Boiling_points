# Boiling_points
the boiling points for all the elements
"""
Element boiling point extension for periodictable in Celsius
source https://en.wikipedia.org/wiki/Boiling_points_of_the_elements_(data_page)
mainly Haynes, William M., ed. (2011). CRC Handbook of Chemistry and Physics (92nd ed.). CRC Press. pp. 4.121-4.123. ISBN 1439855110.
Example --> print U melting temperature in Celsius
>>> import boiling_point
>>> import periodictable as pt
>>> print pt.U.boiling_point

"""
import periodictable.core

def init(table, reload=False):
		if 'boiling_point' in table.properties and not reload:
				return table.properties.append('boiling_point')

		periodictable.core.boiling_point = None

		periodictable.core.boiling_point_units = 'Celsius'

		for symbol,eldata in data.items():
				el = table.symbol(symbol)
				el.boiling_point = eldata
# Data Table
data = dict(
		n 		=		0.,
		H 		=		−252.879,
		He 		=		−268.928,
		Li 		=		1342.000,
		Be 		=		2469.000,
		#CRC was not available for Be
		B 		=		3927.000,
		C 		=		3825.000,
		N 		=		−195.795,
		O 		=		−182.962,
		F 		=		−188.110,
		Ne 		=		−246.046,
		Na		=		882.940,
		Mg 		=		1090.000,
		Al 		=		2519.000,
		Si 		=		3265.000,
		P 		=		280.500,
		S 		= 		444.600,
		Cl 		=		−34.040,
		Ar 		=		−185.848,
		K 		=		759.000,
		Ca 		=		1484.000,
		Sc 		=		2836.000,
		Ti 		=		3287.000,
		V 		=		3407.000,
		Cr 		=		2671.000,
		Mn 		=		2061.000,
		Fe 		=		2861.000,
		Co 		=		2927.000,
		Ni 		=		2913.000,
		Cu 		=		2562.000,
		Zn 		=		907.000,
		Ga 		=		2204.000,
		Ge 		=		2833.000,
		As 		=		603.000,
		Se 		=		685.000,
		Br 		=		58.800,
		Kr 		=		−153.415,
		Rb 		=		688.000,
		Sr 		=		1377.000,
		Y 		=		3345.000,
		Zr 		=		4409.000,
		Nb 		=		4744.000,
		Mo 		=		4639.000,
		Tc 		=		4265.000,
		Ru 		=		4150.000,
		Rh 		=		3695.000,
		Pd 		=		2963.000,
		Ag 		=		2162.000,
		Cd 		=		767.000,
		In 		=		2072.000,
		Sn 		=		2602.000,
		Sb 		=		1587.000,
		Te 		=		988.000,
		I 		=		184.400,
		Xe 		=		−108.099,
		Cs 		=		671.000,
		Ba 		=		1845.000,
		La 		=		3464.000,
		Ce 		=		3443.000,
		Pr 		=		3520.000,
		Nd 		=		3074.000,
		Pm 		=		3000.000,
		Sm 		=		1794.000,
		Eu 		=		1529.000,
		Gd 		=		3273.000,
		Tb 		=		3230.000,
		Dy		=		2567.000,
		Ho 		=		2700.000,
		Er 		=		2868.000,
		Tm 		=		1950.000,
		Yb 		=		1196.000,
		Lu 		=		3402.000,
		Hf 		=		4603.000,
		Ta 		=		5458.000,
		W 		=		5555.000,
		Re 		=		5596.000,
		Os 		=		5012.000,
		Ir  	=		4428.000,
		Pt 		=		3825.000,
		Au 		=		2856.000,
		Hg 		=		356.730,
		Tl 		=		1473.000,
		Pb 		=		1749.000,
		Bi 		=		1564.000,
		Po 		=		962.000,
		At 		=		337.000,
		Rn 		=		−61.700,
		Fr 		=		 677.000,
		Ra 		=		1737.000,
		Ac 		=		3198.000,
		Th 		=		4788.000,
		Pa 		=		4027.000,
		U 		=		4131.000,
		Np 		=		4000.000,
		Pu 		=		3228.000,
		Am 		=		2011.000,
		Cm 		=		3100.000,
)
