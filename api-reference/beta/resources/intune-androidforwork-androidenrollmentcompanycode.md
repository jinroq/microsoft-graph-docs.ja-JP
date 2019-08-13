---
title: androidEnrollmentCompanyCode リソースの種類
description: トークン、Url、QR コードコンテンツなど、Google の Android 管理 API 経由の登録に使用される、専門分野の登録データを保持するクラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ccc8cd1c1753c844ac5a71f9248f8189dad1e0b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367100"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="e8cd7-103">androidEnrollmentCompanyCode リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8cd7-103">androidEnrollmentCompanyCode resource type</span></span>

> <span data-ttu-id="e8cd7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8cd7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8cd7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8cd7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8cd7-106">トークン、Url、QR コードコンテンツなど、Google の Android 管理 API 経由の登録に使用される、専門分野の登録データを保持するクラス</span><span class="sxs-lookup"><span data-stu-id="e8cd7-106">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="e8cd7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8cd7-107">Properties</span></span>
|<span data-ttu-id="e8cd7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8cd7-108">Property</span></span>|<span data-ttu-id="e8cd7-109">型</span><span class="sxs-lookup"><span data-stu-id="e8cd7-109">Type</span></span>|<span data-ttu-id="e8cd7-110">説明</span><span class="sxs-lookup"><span data-stu-id="e8cd7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8cd7-111">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="e8cd7-111">enrollmentToken</span></span>|<span data-ttu-id="e8cd7-112">String</span><span class="sxs-lookup"><span data-stu-id="e8cd7-112">String</span></span>|<span data-ttu-id="e8cd7-113">ユーザーがデバイスを登録するために使用する登録トークン。</span><span class="sxs-lookup"><span data-stu-id="e8cd7-113">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="e8cd7-114">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="e8cd7-114">qrCodeContent</span></span>|<span data-ttu-id="e8cd7-115">String</span><span class="sxs-lookup"><span data-stu-id="e8cd7-115">String</span></span>|<span data-ttu-id="e8cd7-116">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="e8cd7-116">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="e8cd7-117">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="e8cd7-117">qrCodeImage</span></span>|[<span data-ttu-id="e8cd7-118">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e8cd7-118">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e8cd7-119">トークンの生成された QR コード。</span><span class="sxs-lookup"><span data-stu-id="e8cd7-119">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8cd7-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8cd7-120">Relationships</span></span>
<span data-ttu-id="e8cd7-121">なし</span><span class="sxs-lookup"><span data-stu-id="e8cd7-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8cd7-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8cd7-122">JSON Representation</span></span>
<span data-ttu-id="e8cd7-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8cd7-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```



