Terraform "Hello, World" Example
This folder contains the simplest possible Terraform module—one that just outputs "Hello, World"—to demonstrate how you can use Terratest to write automated tests for your Terraform code.

Check out test/terraform_hello_world_example_test.go to see how you can write automated tests for this simple module.

Note that this module doesn't do anything useful; it's just here to demonstrate the simplest usage pattern for Terratest. For a slightly more complicated example of a Terraform module and the corresponding tests, see terraform-basic-example.

Running this module manually
Install Terraform and make sure it's on your PATH.
Run terraform init.
Run terraform apply.
When you're done, run terraform destroy.
Running automated tests against this module
Install Terraform and make sure it's on your PATH.
Install Golang and make sure this code is checked out into your GOPATH.
cd test
go test -v -run TestTerraformHelloWorldExample