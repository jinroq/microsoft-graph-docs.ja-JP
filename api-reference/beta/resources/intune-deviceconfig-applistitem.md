---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 523944b68f899c770569c7e10fea539de2788f7a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333913"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="46f84-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="46f84-103">appListItem resource type</span></span>

> <span data-ttu-id="46f84-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46f84-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46f84-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="46f84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46f84-106">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="46f84-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="46f84-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46f84-107">Properties</span></span>
|<span data-ttu-id="46f84-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46f84-108">Property</span></span>|<span data-ttu-id="46f84-109">型</span><span class="sxs-lookup"><span data-stu-id="46f84-109">Type</span></span>|<span data-ttu-id="46f84-110">説明</span><span class="sxs-lookup"><span data-stu-id="46f84-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46f84-111">name</span><span class="sxs-lookup"><span data-stu-id="46f84-111">name</span></span>|<span data-ttu-id="46f84-112">String</span><span class="sxs-lookup"><span data-stu-id="46f84-112">String</span></span>|<span data-ttu-id="46f84-113">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="46f84-113">The application name</span></span>|
|<span data-ttu-id="46f84-114">発行元</span><span class="sxs-lookup"><span data-stu-id="46f84-114">publisher</span></span>|<span data-ttu-id="46f84-115">String</span><span class="sxs-lookup"><span data-stu-id="46f84-115">String</span></span>|<span data-ttu-id="46f84-116">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="46f84-116">The publisher of the application</span></span>|
|<span data-ttu-id="46f84-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="46f84-117">appStoreUrl</span></span>|<span data-ttu-id="46f84-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="46f84-118">String</span></span>|<span data-ttu-id="46f84-119">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="46f84-119">The Store URL of the application</span></span>|
|<span data-ttu-id="46f84-120">appId</span><span class="sxs-lookup"><span data-stu-id="46f84-120">appId</span></span>|<span data-ttu-id="46f84-121">String</span><span class="sxs-lookup"><span data-stu-id="46f84-121">String</span></span>|<span data-ttu-id="46f84-122">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="46f84-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="46f84-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="46f84-123">Relationships</span></span>
<span data-ttu-id="46f84-124">なし</span><span class="sxs-lookup"><span data-stu-id="46f84-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46f84-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46f84-125">JSON Representation</span></span>
<span data-ttu-id="46f84-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="46f84-126">Here is a JSON representation of the resource.</span></span>
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



