---
title: appConfigurationSettingItem リソースの種類
description: アプリの構成設定アイテムのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2b6b956dcca7ed3540972bae6ff2ba130baaae3f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144493"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="e742b-103">appConfigurationSettingItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e742b-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="e742b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e742b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e742b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e742b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e742b-106">アプリの構成設定アイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e742b-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="e742b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e742b-107">Properties</span></span>
|<span data-ttu-id="e742b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e742b-108">Property</span></span>|<span data-ttu-id="e742b-109">型</span><span class="sxs-lookup"><span data-stu-id="e742b-109">Type</span></span>|<span data-ttu-id="e742b-110">説明</span><span class="sxs-lookup"><span data-stu-id="e742b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e742b-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="e742b-111">appConfigKey</span></span>|<span data-ttu-id="e742b-112">String</span><span class="sxs-lookup"><span data-stu-id="e742b-112">String</span></span>|<span data-ttu-id="e742b-113">アプリの構成キー。</span><span class="sxs-lookup"><span data-stu-id="e742b-113">app configuration key.</span></span>|
|<span data-ttu-id="e742b-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="e742b-114">appConfigKeyType</span></span>|[<span data-ttu-id="e742b-115">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="e742b-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="e742b-116">アプリの構成キーの種類。</span><span class="sxs-lookup"><span data-stu-id="e742b-116">app configuration key type.</span></span> <span data-ttu-id="e742b-117">可能な値は、`stringType`、`integerType`、`realType`、`booleanType`、`tokenType` です。</span><span class="sxs-lookup"><span data-stu-id="e742b-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="e742b-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="e742b-118">appConfigKeyValue</span></span>|<span data-ttu-id="e742b-119">String</span><span class="sxs-lookup"><span data-stu-id="e742b-119">String</span></span>|<span data-ttu-id="e742b-120">アプリの構成キーの値。</span><span class="sxs-lookup"><span data-stu-id="e742b-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e742b-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e742b-121">Relationships</span></span>
<span data-ttu-id="e742b-122">なし</span><span class="sxs-lookup"><span data-stu-id="e742b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e742b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e742b-123">JSON Representation</span></span>
<span data-ttu-id="e742b-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e742b-124">Here is a JSON representation of the resource.</span></span>
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




