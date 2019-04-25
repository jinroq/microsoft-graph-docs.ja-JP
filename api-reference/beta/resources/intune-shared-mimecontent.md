---
title: mimeContent リソースの種類
description: 汎用 MIME コンテンツのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad580548e3f399a3c35d4f86e23eaab4dfa62979
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521265"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="94ec0-103">mimeContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="94ec0-103">mimeContent resource type</span></span>

> <span data-ttu-id="94ec0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94ec0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94ec0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="94ec0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94ec0-106">汎用 MIME コンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="94ec0-106">Contains properties for a generic mime content.</span></span>

## <a name="properties"></a><span data-ttu-id="94ec0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94ec0-107">Properties</span></span>
|<span data-ttu-id="94ec0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94ec0-108">Property</span></span>|<span data-ttu-id="94ec0-109">型</span><span class="sxs-lookup"><span data-stu-id="94ec0-109">Type</span></span>|<span data-ttu-id="94ec0-110">説明</span><span class="sxs-lookup"><span data-stu-id="94ec0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94ec0-111">type</span><span class="sxs-lookup"><span data-stu-id="94ec0-111">type</span></span>|<span data-ttu-id="94ec0-112">String</span><span class="sxs-lookup"><span data-stu-id="94ec0-112">String</span></span>|<span data-ttu-id="94ec0-113">コンテンツ MIME の種類を示します。</span><span class="sxs-lookup"><span data-stu-id="94ec0-113">Indicates the content mime type.</span></span>|
|<span data-ttu-id="94ec0-114">value</span><span class="sxs-lookup"><span data-stu-id="94ec0-114">value</span></span>|<span data-ttu-id="94ec0-115">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="94ec0-115">Binary</span></span>|<span data-ttu-id="94ec0-116">実際のコンテンツを含むバイト配列です。</span><span class="sxs-lookup"><span data-stu-id="94ec0-116">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94ec0-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="94ec0-117">Relationships</span></span>
<span data-ttu-id="94ec0-118">なし</span><span class="sxs-lookup"><span data-stu-id="94ec0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94ec0-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="94ec0-119">JSON Representation</span></span>
<span data-ttu-id="94ec0-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="94ec0-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```





