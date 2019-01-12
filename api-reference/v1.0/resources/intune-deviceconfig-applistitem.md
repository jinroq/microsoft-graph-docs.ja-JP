---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a70f68d291036a7a01823c1946aac655aee6e71c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954429"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="5f3ef-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5f3ef-103">appListItem resource type</span></span>

> <span data-ttu-id="5f3ef-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5f3ef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f3ef-105">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="5f3ef-105">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="5f3ef-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f3ef-106">Properties</span></span>
|<span data-ttu-id="5f3ef-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f3ef-107">Property</span></span>|<span data-ttu-id="5f3ef-108">種類</span><span class="sxs-lookup"><span data-stu-id="5f3ef-108">Type</span></span>|<span data-ttu-id="5f3ef-109">説明</span><span class="sxs-lookup"><span data-stu-id="5f3ef-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f3ef-110">名前</span><span class="sxs-lookup"><span data-stu-id="5f3ef-110">name</span></span>|<span data-ttu-id="5f3ef-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5f3ef-111">String</span></span>|<span data-ttu-id="5f3ef-112">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="5f3ef-112">The application name</span></span>|
|<span data-ttu-id="5f3ef-113">発行元</span><span class="sxs-lookup"><span data-stu-id="5f3ef-113">publisher</span></span>|<span data-ttu-id="5f3ef-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5f3ef-114">String</span></span>|<span data-ttu-id="5f3ef-115">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="5f3ef-115">The publisher of the application</span></span>|
|<span data-ttu-id="5f3ef-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5f3ef-116">appStoreUrl</span></span>|<span data-ttu-id="5f3ef-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5f3ef-117">String</span></span>|<span data-ttu-id="5f3ef-118">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="5f3ef-118">The Store URL of the application</span></span>|
|<span data-ttu-id="5f3ef-119">appId</span><span class="sxs-lookup"><span data-stu-id="5f3ef-119">appId</span></span>|<span data-ttu-id="5f3ef-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5f3ef-120">String</span></span>|<span data-ttu-id="5f3ef-121">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="5f3ef-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f3ef-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5f3ef-122">Relationships</span></span>
<span data-ttu-id="5f3ef-123">なし</span><span class="sxs-lookup"><span data-stu-id="5f3ef-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5f3ef-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5f3ef-124">JSON Representation</span></span>
<span data-ttu-id="5f3ef-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5f3ef-125">Here is a JSON representation of the resource.</span></span>
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



