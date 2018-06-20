---
swagger: "2.0"
x-collection-name: GSA Per Diem API
x-complete: 1
info:
  title: GSA Per Diem API
  description: per-diem-rates-are-the-allowed-reimbursement-rates-for-hotel-stays-and-meals-for-federal-travelers--rates-are-set-for-each-of-the-federal-governments-fiscal-years-fy-2014-is-october-1-2013-to-september-30-2014--gsa-is-responsible-for-setting-the-rates-in-the-continental-united-states---many-businesses-and-other-organizations-adopt-these-rates-as-well--gsa-is-making-the-rates-available-using-the-ckans-action-api-via-data-gov-to-allow-software-developers-programmatic-access-the-data-and-create-innovative-uses-for-it-
  version: 1.0.0
host: inventory.data.gov
basePath: /api/action/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /datastore_search?resource_id=8ea44bc4-22ba-4386-b84c-1494ab28964b:
    get:
      summary: Per Diem Rates
      description: GSA sets rates for geographic areas it determines called primary
        destinations. Areas outside the primary destinations are covered by the same,
        nation-wide standard rate.
      operationId: getPerDiemRates
      x-api-path-slug: datastore-searchresource-id8ea44bc422ba4386b84c1494ab28964b-get
      parameters:
      - in: query
        name: filters
        description: FiscalYear, Zip, State, DestinationID, City, County, Month, Meals
        type: string
        format: string
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
        200:
          description: OK
      tags:
      - Per Diem Rates
---