# WCPFC Geographical Areas

A repository of WKT definitions for the key WCPFC geographical areas including EEZ boundaries and high seas areas within the WCPFC Convention Area

Each file consists of the metadata for each area and a WKT definition of the boundary.

In most cases the boundaries are in the 0-360 longitude range to display on a WGS84 projected map.

To update the spatial definition in SQL Server use the following SQL code:
`UPDATE Geographical_Area SET GAR_Polygon = geography::STPolyFromText('[WKT]',4326).ReorientObject() WHERE GAR_ID = [ID]`
