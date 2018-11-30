---
title: appConfigurationSettingItem リソースの種類
description: アプリの構成設定アイテムのプロパティが含まれています。
ms.openlocfilehash: bd08b325fd04e8e4a742da515d052d453cfb58a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022023"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="47f93-103">appConfigurationSettingItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="47f93-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="47f93-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="47f93-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47f93-105">アプリの構成設定アイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="47f93-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="47f93-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47f93-106">Properties</span></span>
|<span data-ttu-id="47f93-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47f93-107">Property</span></span>|<span data-ttu-id="47f93-108">型</span><span class="sxs-lookup"><span data-stu-id="47f93-108">Type</span></span>|<span data-ttu-id="47f93-109">説明</span><span class="sxs-lookup"><span data-stu-id="47f93-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47f93-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="47f93-110">appConfigKey</span></span>|<span data-ttu-id="47f93-111">String</span><span class="sxs-lookup"><span data-stu-id="47f93-111">String</span></span>|<span data-ttu-id="47f93-112">アプリの構成キー。</span><span class="sxs-lookup"><span data-stu-id="47f93-112">app configuration key.</span></span>|
|<span data-ttu-id="47f93-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="47f93-113">appConfigKeyType</span></span>|[<span data-ttu-id="47f93-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="47f93-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="47f93-115">アプリの構成キーの種類。</span><span class="sxs-lookup"><span data-stu-id="47f93-115">app configuration key type.</span></span> <span data-ttu-id="47f93-116">可能な値は、`stringType`、`integerType`、`realType`、`booleanType`、`tokenType` です。</span><span class="sxs-lookup"><span data-stu-id="47f93-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="47f93-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="47f93-117">appConfigKeyValue</span></span>|<span data-ttu-id="47f93-118">String</span><span class="sxs-lookup"><span data-stu-id="47f93-118">String</span></span>|<span data-ttu-id="47f93-119">アプリの構成キーの値。</span><span class="sxs-lookup"><span data-stu-id="47f93-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47f93-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="47f93-120">Relationships</span></span>
<span data-ttu-id="47f93-121">なし</span><span class="sxs-lookup"><span data-stu-id="47f93-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47f93-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47f93-122">JSON Representation</span></span>
<span data-ttu-id="47f93-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="47f93-123">Here is a JSON representation of the resource.</span></span>
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



