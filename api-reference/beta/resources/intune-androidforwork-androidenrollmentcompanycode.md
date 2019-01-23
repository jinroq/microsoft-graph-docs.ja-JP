---
title: androidEnrollmentCompanyCode リソースの種類
description: トークン、Url、QR コードとコンテンツなど、Google の Android の管理 API を使用して登録するのに使用される専門分野の登録データを保持するクラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be5b2a94445e95fe18271467b6661320d8204d76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430285"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="fa54b-103">androidEnrollmentCompanyCode リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa54b-103">androidEnrollmentCompanyCode resource type</span></span>

> <span data-ttu-id="fa54b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fa54b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fa54b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa54b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa54b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fa54b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa54b-107">トークン、Url、QR コードとコンテンツなど、Google の Android の管理 API を使用して登録するのに使用される専門分野の登録データを保持するクラス</span><span class="sxs-lookup"><span data-stu-id="fa54b-107">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="fa54b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa54b-108">Properties</span></span>
|<span data-ttu-id="fa54b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa54b-109">Property</span></span>|<span data-ttu-id="fa54b-110">型</span><span class="sxs-lookup"><span data-stu-id="fa54b-110">Type</span></span>|<span data-ttu-id="fa54b-111">説明</span><span class="sxs-lookup"><span data-stu-id="fa54b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa54b-112">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="fa54b-112">enrollmentToken</span></span>|<span data-ttu-id="fa54b-113">String</span><span class="sxs-lookup"><span data-stu-id="fa54b-113">String</span></span>|<span data-ttu-id="fa54b-114">登録トークンがそのデバイスを登録するユーザーが使用します。</span><span class="sxs-lookup"><span data-stu-id="fa54b-114">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="fa54b-115">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="fa54b-115">qrCodeContent</span></span>|<span data-ttu-id="fa54b-116">String</span><span class="sxs-lookup"><span data-stu-id="fa54b-116">String</span></span>|<span data-ttu-id="fa54b-117">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="fa54b-117">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="fa54b-118">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="fa54b-118">qrCodeImage</span></span>|[<span data-ttu-id="fa54b-119">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fa54b-119">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fa54b-120">トークンの生成された QR コードです。</span><span class="sxs-lookup"><span data-stu-id="fa54b-120">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa54b-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fa54b-121">Relationships</span></span>
<span data-ttu-id="fa54b-122">なし</span><span class="sxs-lookup"><span data-stu-id="fa54b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa54b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa54b-123">JSON Representation</span></span>
<span data-ttu-id="fa54b-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fa54b-124">Here is a JSON representation of the resource.</span></span>
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




