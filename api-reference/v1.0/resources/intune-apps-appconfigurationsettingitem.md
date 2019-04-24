---
title: appConfigurationSettingItem リソースの種類
description: アプリの構成設定アイテムのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 11ef3a964d166301c04c49730ac084b68e700b7c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503591"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="bf615-103">appConfigurationSettingItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf615-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="bf615-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bf615-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf615-105">アプリの構成設定アイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bf615-105">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="bf615-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf615-106">Properties</span></span>
|<span data-ttu-id="bf615-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf615-107">Property</span></span>|<span data-ttu-id="bf615-108">型</span><span class="sxs-lookup"><span data-stu-id="bf615-108">Type</span></span>|<span data-ttu-id="bf615-109">説明</span><span class="sxs-lookup"><span data-stu-id="bf615-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf615-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="bf615-110">appConfigKey</span></span>|<span data-ttu-id="bf615-111">String</span><span class="sxs-lookup"><span data-stu-id="bf615-111">String</span></span>|<span data-ttu-id="bf615-112">アプリの構成キー。</span><span class="sxs-lookup"><span data-stu-id="bf615-112">app configuration key.</span></span>|
|<span data-ttu-id="bf615-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="bf615-113">appConfigKeyType</span></span>|[<span data-ttu-id="bf615-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="bf615-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="bf615-115">アプリの構成キーの種類。</span><span class="sxs-lookup"><span data-stu-id="bf615-115">app configuration key type.</span></span> <span data-ttu-id="bf615-116">可能な値は、`stringType`、`integerType`、`realType`、`booleanType`、`tokenType` です。</span><span class="sxs-lookup"><span data-stu-id="bf615-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="bf615-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="bf615-117">appConfigKeyValue</span></span>|<span data-ttu-id="bf615-118">String</span><span class="sxs-lookup"><span data-stu-id="bf615-118">String</span></span>|<span data-ttu-id="bf615-119">アプリの構成キーの値。</span><span class="sxs-lookup"><span data-stu-id="bf615-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf615-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bf615-120">Relationships</span></span>
<span data-ttu-id="bf615-121">なし</span><span class="sxs-lookup"><span data-stu-id="bf615-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf615-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf615-122">JSON Representation</span></span>
<span data-ttu-id="bf615-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf615-123">Here is a JSON representation of the resource.</span></span>
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



