---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
author: tfitzmac
ms.openlocfilehash: a7e33b986f95f610abff2c7b5321f48f3668e488
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323598"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="b0f27-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0f27-103">appListItem resource type</span></span>

> <span data-ttu-id="b0f27-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0f27-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0f27-105">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="b0f27-105">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="b0f27-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0f27-106">Properties</span></span>
|<span data-ttu-id="b0f27-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0f27-107">Property</span></span>|<span data-ttu-id="b0f27-108">種類</span><span class="sxs-lookup"><span data-stu-id="b0f27-108">Type</span></span>|<span data-ttu-id="b0f27-109">説明</span><span class="sxs-lookup"><span data-stu-id="b0f27-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0f27-110">名前</span><span class="sxs-lookup"><span data-stu-id="b0f27-110">name</span></span>|<span data-ttu-id="b0f27-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0f27-111">String</span></span>|<span data-ttu-id="b0f27-112">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="b0f27-112">The application name</span></span>|
|<span data-ttu-id="b0f27-113">発行元</span><span class="sxs-lookup"><span data-stu-id="b0f27-113">publisher</span></span>|<span data-ttu-id="b0f27-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0f27-114">String</span></span>|<span data-ttu-id="b0f27-115">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="b0f27-115">The publisher of the application</span></span>|
|<span data-ttu-id="b0f27-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b0f27-116">appStoreUrl</span></span>|<span data-ttu-id="b0f27-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0f27-117">String</span></span>|<span data-ttu-id="b0f27-118">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="b0f27-118">The Store URL of the application</span></span>|
|<span data-ttu-id="b0f27-119">appId</span><span class="sxs-lookup"><span data-stu-id="b0f27-119">appId</span></span>|<span data-ttu-id="b0f27-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0f27-120">String</span></span>|<span data-ttu-id="b0f27-121">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="b0f27-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0f27-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b0f27-122">Relationships</span></span>
<span data-ttu-id="b0f27-123">なし</span><span class="sxs-lookup"><span data-stu-id="b0f27-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b0f27-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0f27-124">JSON Representation</span></span>
<span data-ttu-id="b0f27-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b0f27-125">Here is a JSON representation of the resource.</span></span>
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



