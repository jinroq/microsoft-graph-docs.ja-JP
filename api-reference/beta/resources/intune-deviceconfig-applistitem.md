---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d29fca9155ac14c7b8ebf9ad862bda3bed874353
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947716"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="00d16-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="00d16-103">appListItem resource type</span></span>

> <span data-ttu-id="00d16-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00d16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00d16-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="00d16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00d16-106">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="00d16-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="00d16-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00d16-107">Properties</span></span>
|<span data-ttu-id="00d16-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00d16-108">Property</span></span>|<span data-ttu-id="00d16-109">型</span><span class="sxs-lookup"><span data-stu-id="00d16-109">Type</span></span>|<span data-ttu-id="00d16-110">説明</span><span class="sxs-lookup"><span data-stu-id="00d16-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00d16-111">name</span><span class="sxs-lookup"><span data-stu-id="00d16-111">name</span></span>|<span data-ttu-id="00d16-112">String</span><span class="sxs-lookup"><span data-stu-id="00d16-112">String</span></span>|<span data-ttu-id="00d16-113">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="00d16-113">The application name</span></span>|
|<span data-ttu-id="00d16-114">発行元</span><span class="sxs-lookup"><span data-stu-id="00d16-114">publisher</span></span>|<span data-ttu-id="00d16-115">String</span><span class="sxs-lookup"><span data-stu-id="00d16-115">String</span></span>|<span data-ttu-id="00d16-116">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="00d16-116">The publisher of the application</span></span>|
|<span data-ttu-id="00d16-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="00d16-117">appStoreUrl</span></span>|<span data-ttu-id="00d16-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="00d16-118">String</span></span>|<span data-ttu-id="00d16-119">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="00d16-119">The Store URL of the application</span></span>|
|<span data-ttu-id="00d16-120">appId</span><span class="sxs-lookup"><span data-stu-id="00d16-120">appId</span></span>|<span data-ttu-id="00d16-121">String</span><span class="sxs-lookup"><span data-stu-id="00d16-121">String</span></span>|<span data-ttu-id="00d16-122">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="00d16-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="00d16-123">関係</span><span class="sxs-lookup"><span data-stu-id="00d16-123">Relationships</span></span>
<span data-ttu-id="00d16-124">なし</span><span class="sxs-lookup"><span data-stu-id="00d16-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00d16-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="00d16-125">JSON Representation</span></span>
<span data-ttu-id="00d16-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="00d16-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```




