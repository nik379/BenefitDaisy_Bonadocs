﻿## BenefitDaisy


### Campaign

```solidity
struct Campaign {
  string title;
  string description;
  address owner;
  uint256 deadline;
  uint256 target;
  uint256 amountCollected;
  string image;
  address[] donators;
  uint256[] donations;
}
```
### campaigns

```solidity
mapping(uint256 => struct BenefitDaisy.Campaign) campaigns
```

### numberOfCampaigns

```solidity
uint256 numberOfCampaigns
```

### createCampaign

```solidity
function createCampaign(address _owner, string _title, string _description, uint256 _target, uint256 _deadline, string _image) public returns (uint256)
```







### donateToCamapign

```solidity
function donateToCamapign(uint256 _id) public payable
```







### getDonators

```solidity
function getDonators(uint256 _id) public view returns (address[], uint256[])
```







### getCampaigns

```solidity
function getCampaigns() public view returns (struct BenefitDaisy.Campaign[])
```







