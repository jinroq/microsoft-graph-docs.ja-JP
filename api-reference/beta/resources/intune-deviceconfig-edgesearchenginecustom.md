---
title: edgeSearchEngineCustom リソースの種類
description: IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。
ms.openlocfilehash: 5312f53e43921d71e6c338ccb112a851773abc43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069536"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="f9f59-103">edgeSearchEngineCustom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f9f59-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="f9f59-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f9f59-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9f59-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9f59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9f59-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f9f59-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9f59-107">IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="f9f59-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="f9f59-108">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f9f59-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f9f59-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9f59-109">Properties</span></span>
|<span data-ttu-id="f9f59-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9f59-110">Property</span></span>|<span data-ttu-id="f9f59-111">型</span><span class="sxs-lookup"><span data-stu-id="f9f59-111">Type</span></span>|<span data-ttu-id="f9f59-112">説明</span><span class="sxs-lookup"><span data-stu-id="f9f59-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9f59-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="f9f59-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="f9f59-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f9f59-114">String</span></span>|<span data-ttu-id="f9f59-115">短縮名と検索エンジンの URL が最低限含まれる OpenSearch xml ファイルが入っている https リンクを指します。</span><span class="sxs-lookup"><span data-stu-id="f9f59-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9f59-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f9f59-116">Relationships</span></span>
<span data-ttu-id="f9f59-117">なし</span><span class="sxs-lookup"><span data-stu-id="f9f59-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f9f59-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f9f59-118">JSON Representation</span></span>
<span data-ttu-id="f9f59-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f9f59-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```





