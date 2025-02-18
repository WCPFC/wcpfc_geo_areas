# WCPFC Geographical Areas

A repository of WKT definitions for the key WCPFC geographical areas including EEZ boundaries and high seas areas within the WCPFC Convention Area

Each file consists to the metadata for each area and a WKT definition of the boundary.

To update the spatial definition in SQL Server use the following SQL code:
`UPDATE Geographical_Area SET GAR_Polygon = geography::STPolyFromText('[WKT]',4326) WHERE GAR_ID = [ID]`
