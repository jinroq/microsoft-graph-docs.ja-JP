---
title: appConfigurationSettingItem リソースの種類
description: アプリの構成設定アイテムのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddd574ea19057fe31dbca5f258f8153071cd440c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927129"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="2be0b-103">appConfigurationSettingItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2be0b-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="2be0b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2be0b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2be0b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2be0b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2be0b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2be0b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2be0b-107">アプリの構成設定アイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2be0b-107">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="2be0b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2be0b-108">Properties</span></span>
|<span data-ttu-id="2be0b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2be0b-109">Property</span></span>|<span data-ttu-id="2be0b-110">種類</span><span class="sxs-lookup"><span data-stu-id="2be0b-110">Type</span></span>|<span data-ttu-id="2be0b-111">説明</span><span class="sxs-lookup"><span data-stu-id="2be0b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2be0b-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="2be0b-112">appConfigKey</span></span>|<span data-ttu-id="2be0b-113">String</span><span class="sxs-lookup"><span data-stu-id="2be0b-113">String</span></span>|<span data-ttu-id="2be0b-114">アプリの構成キー。</span><span class="sxs-lookup"><span data-stu-id="2be0b-114">app configuration key.</span></span>|
|<span data-ttu-id="2be0b-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="2be0b-115">appConfigKeyType</span></span>|[<span data-ttu-id="2be0b-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="2be0b-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="2be0b-117">アプリの構成キーの種類。</span><span class="sxs-lookup"><span data-stu-id="2be0b-117">app configuration key type.</span></span> <span data-ttu-id="2be0b-118">可能な値は、`stringType`、`integerType`、`realType`、`booleanType`、`tokenType` です。</span><span class="sxs-lookup"><span data-stu-id="2be0b-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="2be0b-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="2be0b-119">appConfigKeyValue</span></span>|<span data-ttu-id="2be0b-120">String</span><span class="sxs-lookup"><span data-stu-id="2be0b-120">String</span></span>|<span data-ttu-id="2be0b-121">アプリの構成キーの値。</span><span class="sxs-lookup"><span data-stu-id="2be0b-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2be0b-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2be0b-122">Relationships</span></span>
<span data-ttu-id="2be0b-123">なし</span><span class="sxs-lookup"><span data-stu-id="2be0b-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2be0b-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2be0b-124">JSON Representation</span></span>
<span data-ttu-id="2be0b-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2be0b-125">Here is a JSON representation of the resource.</span></span>
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





