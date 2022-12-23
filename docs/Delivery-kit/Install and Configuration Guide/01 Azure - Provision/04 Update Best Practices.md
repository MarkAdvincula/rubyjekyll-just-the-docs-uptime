# Update Best Practices

## Updating the fork from remote branch

1. Click 'Fetch Upstream', and click 'Fetch and Merge'. You can also check the comparisons to check any changes made from the remote vs forked branch.  
<i>Note: Fetch Upstream only updates the current branch you fetched</i>
![best-practices](../../../assets/images/delivery-kit/update-repository.png)

2. Once done, the build pipelines on DevOps will automatically update. You can check it on Azure DevOps as well, where the related repository is in the build pipeline.

3. If the build goes successful, go to Releases branch and Create a release, and select the version you want to deploy. The steps can be found at [Azure DevOps](https://github.dxc.com/WorkplaceAndMobility/DXC-MW-UPT/blob/R2-Delivery-Kit/content/Delivery-Kit/Installation%20and%20Configuration%20Guide/01%20Azure%20-%20Provision/01%20Azure%20DevOps.md) at section Releases, #4.

