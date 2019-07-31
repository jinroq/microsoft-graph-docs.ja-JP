---
title: appConfigurationSettingItem リソースの種類
description: アプリの構成設定アイテムのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c001e19758865e957cb3d72f3d49acf3387281a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006053"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="a3e34-103">appConfigurationSettingItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a3e34-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="a3e34-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3e34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3e34-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3e34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3e34-106">アプリの構成設定アイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a3e34-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="a3e34-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3e34-107">Properties</span></span>
|<span data-ttu-id="a3e34-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3e34-108">Property</span></span>|<span data-ttu-id="a3e34-109">型</span><span class="sxs-lookup"><span data-stu-id="a3e34-109">Type</span></span>|<span data-ttu-id="a3e34-110">説明</span><span class="sxs-lookup"><span data-stu-id="a3e34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3e34-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="a3e34-111">appConfigKey</span></span>|<span data-ttu-id="a3e34-112">String</span><span class="sxs-lookup"><span data-stu-id="a3e34-112">String</span></span>|<span data-ttu-id="a3e34-113">アプリの構成キー。</span><span class="sxs-lookup"><span data-stu-id="a3e34-113">app configuration key.</span></span>|
|<span data-ttu-id="a3e34-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="a3e34-114">appConfigKeyType</span></span>|[<span data-ttu-id="a3e34-115">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="a3e34-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="a3e34-116">アプリの構成キーの種類。</span><span class="sxs-lookup"><span data-stu-id="a3e34-116">app configuration key type.</span></span> <span data-ttu-id="a3e34-117">可能な値は、`stringType`、`integerType`、`realType`、`booleanType`、`tokenType` です。</span><span class="sxs-lookup"><span data-stu-id="a3e34-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="a3e34-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="a3e34-118">appConfigKeyValue</span></span>|<span data-ttu-id="a3e34-119">String</span><span class="sxs-lookup"><span data-stu-id="a3e34-119">String</span></span>|<span data-ttu-id="a3e34-120">アプリの構成キーの値。</span><span class="sxs-lookup"><span data-stu-id="a3e34-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3e34-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a3e34-121">Relationships</span></span>
<span data-ttu-id="a3e34-122">なし</span><span class="sxs-lookup"><span data-stu-id="a3e34-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3e34-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a3e34-123">JSON Representation</span></span>
<span data-ttu-id="a3e34-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a3e34-124">Here is a JSON representation of the resource.</span></span>
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





