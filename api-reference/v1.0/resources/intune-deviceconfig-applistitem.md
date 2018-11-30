---
title: appListItem リソースの種類
description: 管理対象アプリケーションの一覧にあるアプリを表します
ms.openlocfilehash: c9b39b5fdee8bb503ef66f729a6ee478581a6391
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020827"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="09593-103">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09593-103">appListItem resource type</span></span>

> <span data-ttu-id="09593-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="09593-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09593-105">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="09593-105">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="09593-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09593-106">Properties</span></span>
|<span data-ttu-id="09593-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09593-107">Property</span></span>|<span data-ttu-id="09593-108">型</span><span class="sxs-lookup"><span data-stu-id="09593-108">Type</span></span>|<span data-ttu-id="09593-109">説明</span><span class="sxs-lookup"><span data-stu-id="09593-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09593-110">名前</span><span class="sxs-lookup"><span data-stu-id="09593-110">name</span></span>|<span data-ttu-id="09593-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="09593-111">String</span></span>|<span data-ttu-id="09593-112">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="09593-112">The application name</span></span>|
|<span data-ttu-id="09593-113">発行元</span><span class="sxs-lookup"><span data-stu-id="09593-113">publisher</span></span>|<span data-ttu-id="09593-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="09593-114">String</span></span>|<span data-ttu-id="09593-115">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="09593-115">The publisher of the application</span></span>|
|<span data-ttu-id="09593-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="09593-116">appStoreUrl</span></span>|<span data-ttu-id="09593-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="09593-117">String</span></span>|<span data-ttu-id="09593-118">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="09593-118">The Store URL of the application</span></span>|
|<span data-ttu-id="09593-119">appId</span><span class="sxs-lookup"><span data-stu-id="09593-119">appId</span></span>|<span data-ttu-id="09593-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="09593-120">String</span></span>|<span data-ttu-id="09593-121">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="09593-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="09593-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09593-122">Relationships</span></span>
<span data-ttu-id="09593-123">なし</span><span class="sxs-lookup"><span data-stu-id="09593-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09593-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09593-124">JSON Representation</span></span>
<span data-ttu-id="09593-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09593-125">Here is a JSON representation of the resource.</span></span>
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



