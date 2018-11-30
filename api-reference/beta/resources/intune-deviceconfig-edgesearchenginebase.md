---
title: edgeSearchEngineBase リソースの種類
description: IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。 AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。
ms.openlocfilehash: b6f006d1bdedc2b6fafaf29565fff6b3dcbb0a5b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071694"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="39854-104">edgeSearchEngineBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39854-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="39854-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="39854-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39854-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39854-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39854-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="39854-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39854-108">IT 管理者が MDM 制御デバイス用の既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="39854-108">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="39854-109">AllowSearchEngineCustomization ポリシーが設定されていない場合、ユーザーは上書きして既定の検索エンジンを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="39854-109">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="39854-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39854-110">Properties</span></span>
|<span data-ttu-id="39854-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39854-111">Property</span></span>|<span data-ttu-id="39854-112">型</span><span class="sxs-lookup"><span data-stu-id="39854-112">Type</span></span>|<span data-ttu-id="39854-113">説明</span><span class="sxs-lookup"><span data-stu-id="39854-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="39854-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39854-114">Relationships</span></span>
<span data-ttu-id="39854-115">なし</span><span class="sxs-lookup"><span data-stu-id="39854-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39854-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39854-116">JSON Representation</span></span>
<span data-ttu-id="39854-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39854-117">Here is a JSON representation of the resource.</span></span>
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





