---
title: androidEnrollmentCompanyCode リソースの種類
description: トークン、Url、QR コードコンテンツなど、Google の Android 管理 API 経由の登録に使用される、専門分野の登録データを保持するクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0422bf09d990c02c984b45fa144d6ae12661f718
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552801"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="e2deb-103">androidEnrollmentCompanyCode リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2deb-103">androidEnrollmentCompanyCode resource type</span></span>

> <span data-ttu-id="e2deb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2deb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2deb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e2deb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2deb-106">トークン、Url、QR コードコンテンツなど、Google の Android 管理 API 経由の登録に使用される、専門分野の登録データを保持するクラス</span><span class="sxs-lookup"><span data-stu-id="e2deb-106">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="e2deb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2deb-107">Properties</span></span>
|<span data-ttu-id="e2deb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2deb-108">Property</span></span>|<span data-ttu-id="e2deb-109">型</span><span class="sxs-lookup"><span data-stu-id="e2deb-109">Type</span></span>|<span data-ttu-id="e2deb-110">説明</span><span class="sxs-lookup"><span data-stu-id="e2deb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2deb-111">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="e2deb-111">enrollmentToken</span></span>|<span data-ttu-id="e2deb-112">String</span><span class="sxs-lookup"><span data-stu-id="e2deb-112">String</span></span>|<span data-ttu-id="e2deb-113">ユーザーがデバイスを登録するために使用する登録トークン。</span><span class="sxs-lookup"><span data-stu-id="e2deb-113">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="e2deb-114">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="e2deb-114">qrCodeContent</span></span>|<span data-ttu-id="e2deb-115">String</span><span class="sxs-lookup"><span data-stu-id="e2deb-115">String</span></span>|<span data-ttu-id="e2deb-116">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="e2deb-116">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="e2deb-117">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="e2deb-117">qrCodeImage</span></span>|[<span data-ttu-id="e2deb-118">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e2deb-118">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e2deb-119">トークンの生成された QR コード。</span><span class="sxs-lookup"><span data-stu-id="e2deb-119">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2deb-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e2deb-120">Relationships</span></span>
<span data-ttu-id="e2deb-121">なし</span><span class="sxs-lookup"><span data-stu-id="e2deb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2deb-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2deb-122">JSON Representation</span></span>
<span data-ttu-id="e2deb-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e2deb-123">Here is a JSON representation of the resource.</span></span>
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





