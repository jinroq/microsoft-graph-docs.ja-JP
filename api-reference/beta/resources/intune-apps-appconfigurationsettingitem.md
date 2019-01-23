---
title: appConfigurationSettingItem リソースの種類
description: アプリの構成設定アイテムのプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7f5492c9b54c9414db6a8332e218a1d7f0a50b1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403764"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="a89ab-103">appConfigurationSettingItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a89ab-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="a89ab-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a89ab-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a89ab-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a89ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a89ab-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a89ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a89ab-107">アプリの構成設定アイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a89ab-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="a89ab-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a89ab-108">Properties</span></span>
|<span data-ttu-id="a89ab-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a89ab-109">Property</span></span>|<span data-ttu-id="a89ab-110">型</span><span class="sxs-lookup"><span data-stu-id="a89ab-110">Type</span></span>|<span data-ttu-id="a89ab-111">説明</span><span class="sxs-lookup"><span data-stu-id="a89ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a89ab-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="a89ab-112">appConfigKey</span></span>|<span data-ttu-id="a89ab-113">String</span><span class="sxs-lookup"><span data-stu-id="a89ab-113">String</span></span>|<span data-ttu-id="a89ab-114">アプリの構成キー。</span><span class="sxs-lookup"><span data-stu-id="a89ab-114">app configuration key.</span></span>|
|<span data-ttu-id="a89ab-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="a89ab-115">appConfigKeyType</span></span>|[<span data-ttu-id="a89ab-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="a89ab-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="a89ab-117">アプリの構成キーの種類。</span><span class="sxs-lookup"><span data-stu-id="a89ab-117">app configuration key type.</span></span> <span data-ttu-id="a89ab-118">可能な値は、`stringType`、`integerType`、`realType`、`booleanType`、`tokenType` です。</span><span class="sxs-lookup"><span data-stu-id="a89ab-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="a89ab-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="a89ab-119">appConfigKeyValue</span></span>|<span data-ttu-id="a89ab-120">String</span><span class="sxs-lookup"><span data-stu-id="a89ab-120">String</span></span>|<span data-ttu-id="a89ab-121">アプリの構成キーの値。</span><span class="sxs-lookup"><span data-stu-id="a89ab-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a89ab-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a89ab-122">Relationships</span></span>
<span data-ttu-id="a89ab-123">なし</span><span class="sxs-lookup"><span data-stu-id="a89ab-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a89ab-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a89ab-124">JSON Representation</span></span>
<span data-ttu-id="a89ab-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a89ab-125">Here is a JSON representation of the resource.</span></span>
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




