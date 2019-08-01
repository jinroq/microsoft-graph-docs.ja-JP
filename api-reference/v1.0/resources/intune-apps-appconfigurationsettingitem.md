---
title: appConfigurationSettingItem リソースの種類
description: アプリの構成設定アイテムのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91ccefc06ba6a635b9b18e07465ea0332c48f022
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030178"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="b81d4-103">appConfigurationSettingItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b81d4-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="b81d4-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b81d4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b81d4-105">アプリの構成設定アイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b81d4-105">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="b81d4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b81d4-106">Properties</span></span>
|<span data-ttu-id="b81d4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b81d4-107">Property</span></span>|<span data-ttu-id="b81d4-108">型</span><span class="sxs-lookup"><span data-stu-id="b81d4-108">Type</span></span>|<span data-ttu-id="b81d4-109">説明</span><span class="sxs-lookup"><span data-stu-id="b81d4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b81d4-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="b81d4-110">appConfigKey</span></span>|<span data-ttu-id="b81d4-111">String</span><span class="sxs-lookup"><span data-stu-id="b81d4-111">String</span></span>|<span data-ttu-id="b81d4-112">アプリの構成キー。</span><span class="sxs-lookup"><span data-stu-id="b81d4-112">app configuration key.</span></span>|
|<span data-ttu-id="b81d4-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="b81d4-113">appConfigKeyType</span></span>|[<span data-ttu-id="b81d4-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="b81d4-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="b81d4-115">アプリの構成キーの種類。</span><span class="sxs-lookup"><span data-stu-id="b81d4-115">app configuration key type.</span></span> <span data-ttu-id="b81d4-116">可能な値は、`stringType`、`integerType`、`realType`、`booleanType`、`tokenType` です。</span><span class="sxs-lookup"><span data-stu-id="b81d4-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="b81d4-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="b81d4-117">appConfigKeyValue</span></span>|<span data-ttu-id="b81d4-118">String</span><span class="sxs-lookup"><span data-stu-id="b81d4-118">String</span></span>|<span data-ttu-id="b81d4-119">アプリの構成キーの値。</span><span class="sxs-lookup"><span data-stu-id="b81d4-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b81d4-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b81d4-120">Relationships</span></span>
<span data-ttu-id="b81d4-121">なし</span><span class="sxs-lookup"><span data-stu-id="b81d4-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b81d4-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b81d4-122">JSON Representation</span></span>
<span data-ttu-id="b81d4-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b81d4-123">Here is a JSON representation of the resource.</span></span>
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



