# RCA
## DICOMweb
### WADO-RS
url: http://localhost:8080/rest/xxx/studies/uid/series/uid/instances/uid/

1. Accept:	\*/\*
   - RETURN: DICOM UNCOMPRESSED

2. Accept: application/octet-stream
   - RETURN: DICOM NOTHING

3. Accept: application/dicom
   - RETURN: DICOM COMPRESSED

For multipart responses, delete ALL the content up to the first line of the DICOM and from the last byte of the end of the DICOM.
