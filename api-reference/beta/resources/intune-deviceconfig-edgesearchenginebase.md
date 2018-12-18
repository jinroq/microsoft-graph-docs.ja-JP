---
title: edgeSearchEngineBase リソースの種類
description: IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。
author: tfitzmac
ms.openlocfilehash: c60dd1786f5a211947c02f1a9f5f048737ba3788
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346502"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="9f3f4-104">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f3f4-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="9f3f4-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f3f4-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f3f4-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f3f4-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f3f4-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9f3f4-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f3f4-108">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="9f3f4-108">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="9f3f4-109">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="9f3f4-109">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="9f3f4-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f3f4-110">Properties</span></span>
|<span data-ttu-id="9f3f4-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f3f4-111">Property</span></span>|<span data-ttu-id="9f3f4-112">種類</span><span class="sxs-lookup"><span data-stu-id="9f3f4-112">Type</span></span>|<span data-ttu-id="9f3f4-113">説明</span><span class="sxs-lookup"><span data-stu-id="9f3f4-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="9f3f4-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9f3f4-114">Relationships</span></span>
<span data-ttu-id="9f3f4-115">なし</span><span class="sxs-lookup"><span data-stu-id="9f3f4-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9f3f4-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f3f4-116">JSON Representation</span></span>
<span data-ttu-id="9f3f4-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f3f4-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineBase"
}
```





