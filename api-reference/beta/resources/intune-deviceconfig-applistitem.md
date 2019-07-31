---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f985994ae3d69280ac1bd55626096cf6de46adf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971117"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="65b91-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="65b91-103">appListItem resource type</span></span>

> <span data-ttu-id="65b91-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65b91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65b91-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="65b91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65b91-106">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="65b91-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="65b91-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65b91-107">Properties</span></span>
|<span data-ttu-id="65b91-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="65b91-108">Property</span></span>|<span data-ttu-id="65b91-109">型</span><span class="sxs-lookup"><span data-stu-id="65b91-109">Type</span></span>|<span data-ttu-id="65b91-110">説明</span><span class="sxs-lookup"><span data-stu-id="65b91-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65b91-111">name</span><span class="sxs-lookup"><span data-stu-id="65b91-111">name</span></span>|<span data-ttu-id="65b91-112">String</span><span class="sxs-lookup"><span data-stu-id="65b91-112">String</span></span>|<span data-ttu-id="65b91-113">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="65b91-113">The application name</span></span>|
|<span data-ttu-id="65b91-114">発行元</span><span class="sxs-lookup"><span data-stu-id="65b91-114">publisher</span></span>|<span data-ttu-id="65b91-115">String</span><span class="sxs-lookup"><span data-stu-id="65b91-115">String</span></span>|<span data-ttu-id="65b91-116">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="65b91-116">The publisher of the application</span></span>|
|<span data-ttu-id="65b91-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="65b91-117">appStoreUrl</span></span>|<span data-ttu-id="65b91-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="65b91-118">String</span></span>|<span data-ttu-id="65b91-119">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="65b91-119">The Store URL of the application</span></span>|
|<span data-ttu-id="65b91-120">appId</span><span class="sxs-lookup"><span data-stu-id="65b91-120">appId</span></span>|<span data-ttu-id="65b91-121">String</span><span class="sxs-lookup"><span data-stu-id="65b91-121">String</span></span>|<span data-ttu-id="65b91-122">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="65b91-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="65b91-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="65b91-123">Relationships</span></span>
<span data-ttu-id="65b91-124">なし</span><span class="sxs-lookup"><span data-stu-id="65b91-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65b91-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="65b91-125">JSON Representation</span></span>
<span data-ttu-id="65b91-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="65b91-126">Here is a JSON representation of the resource.</span></span>
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





