<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	chaseonboardingtestsamplesdk "github.com/speakeasy-sdks-staging/chase-onboarding-test-sample-sdk"
	"github.com/speakeasy-sdks-staging/chase-onboarding-test-sample-sdk/pkg/models/shared"
	"log"
	"net/http"
)

func main() {
	s := chaseonboardingtestsamplesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx, shared.Pet{
		ID:   596804,
		Name: "string",
	})
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->