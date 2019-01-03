---
title: loggedOnUser リソースの種類
description: ログオン中のユーザー
author: tfitzmac
ms.openlocfilehash: c2021d51356798dec906331797a2504f779264b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327175"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="c20db-103">loggedOnUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c20db-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="c20db-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c20db-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c20db-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c20db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c20db-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c20db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c20db-107">ログオン中のユーザー</span><span class="sxs-lookup"><span data-stu-id="c20db-107">Logged On User</span></span>
## <a name="properties"></a><span data-ttu-id="c20db-108">Properties</span><span class="sxs-lookup"><span data-stu-id="c20db-108">Properties</span></span>
|<span data-ttu-id="c20db-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c20db-109">Property</span></span>|<span data-ttu-id="c20db-110">種類</span><span class="sxs-lookup"><span data-stu-id="c20db-110">Type</span></span>|<span data-ttu-id="c20db-111">説明</span><span class="sxs-lookup"><span data-stu-id="c20db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c20db-112">userId</span><span class="sxs-lookup"><span data-stu-id="c20db-112">userId</span></span>|<span data-ttu-id="c20db-113">String</span><span class="sxs-lookup"><span data-stu-id="c20db-113">String</span></span>|<span data-ttu-id="c20db-114">ユーザー id</span><span class="sxs-lookup"><span data-stu-id="c20db-114">User id</span></span>|
|<span data-ttu-id="c20db-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="c20db-115">lastLogOnDateTime</span></span>|<span data-ttu-id="c20db-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c20db-116">DateTimeOffset</span></span>|<span data-ttu-id="c20db-117">ユーザーのログオン時の日付します。</span><span class="sxs-lookup"><span data-stu-id="c20db-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="c20db-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c20db-118">Relationships</span></span>
<span data-ttu-id="c20db-119">なし</span><span class="sxs-lookup"><span data-stu-id="c20db-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c20db-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c20db-120">JSON Representation</span></span>
<span data-ttu-id="c20db-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c20db-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```




