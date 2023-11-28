<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	chaseonboardingtestsamplesdk "github.com/speakeasy-sdks-staging/chase-onboarding-test-sample-sdk"
	"log"
	"net/http"
)

func main() {
	s := chaseonboardingtestsamplesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->