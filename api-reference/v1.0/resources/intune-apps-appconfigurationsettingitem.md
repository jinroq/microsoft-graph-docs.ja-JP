---
title: appConfigurationSettingItem リソースの種類
description: アプリの構成設定アイテムのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 900a16544b0166263b7d40c428c2c4cbaf5a0bb6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830423"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="5d71d-103">appConfigurationSettingItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5d71d-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="5d71d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5d71d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d71d-105">アプリの構成設定アイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5d71d-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="5d71d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d71d-106">Properties</span></span>
|<span data-ttu-id="5d71d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d71d-107">Property</span></span>|<span data-ttu-id="5d71d-108">種類</span><span class="sxs-lookup"><span data-stu-id="5d71d-108">Type</span></span>|<span data-ttu-id="5d71d-109">説明</span><span class="sxs-lookup"><span data-stu-id="5d71d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d71d-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="5d71d-110">appConfigKey</span></span>|<span data-ttu-id="5d71d-111">String</span><span class="sxs-lookup"><span data-stu-id="5d71d-111">String</span></span>|<span data-ttu-id="5d71d-112">アプリの構成キー。</span><span class="sxs-lookup"><span data-stu-id="5d71d-112">app configuration key.</span></span>|
|<span data-ttu-id="5d71d-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="5d71d-113">appConfigKeyType</span></span>|[<span data-ttu-id="5d71d-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="5d71d-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="5d71d-115">アプリの構成キーの種類。</span><span class="sxs-lookup"><span data-stu-id="5d71d-115">app configuration key type.</span></span> <span data-ttu-id="5d71d-116">可能な値は、`stringType`、`integerType`、`realType`、`booleanType`、`tokenType` です。</span><span class="sxs-lookup"><span data-stu-id="5d71d-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="5d71d-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="5d71d-117">appConfigKeyValue</span></span>|<span data-ttu-id="5d71d-118">String</span><span class="sxs-lookup"><span data-stu-id="5d71d-118">String</span></span>|<span data-ttu-id="5d71d-119">アプリの構成キーの値。</span><span class="sxs-lookup"><span data-stu-id="5d71d-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d71d-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5d71d-120">Relationships</span></span>
<span data-ttu-id="5d71d-121">なし</span><span class="sxs-lookup"><span data-stu-id="5d71d-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5d71d-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5d71d-122">JSON Representation</span></span>
<span data-ttu-id="5d71d-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5d71d-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



