---
title: iosVppEBooks のリスト
description: iosVppEBook オブジェクトのプロパティとリレーションシップをリストします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 470109ed62b0f42d69122f64b49783ecc5b85fca
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420620"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="6f844-103">iosVppEBooks のリスト</span><span class="sxs-lookup"><span data-stu-id="6f844-103">List iosVppEBooks</span></span>

> <span data-ttu-id="6f844-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6f844-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f844-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f844-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f844-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f844-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f844-107">[iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6f844-107">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f844-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6f844-108">Prerequisites</span></span>
<span data-ttu-id="6f844-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f844-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6f844-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6f844-111">Permission type</span></span>|<span data-ttu-id="6f844-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6f844-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f844-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6f844-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f844-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f844-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6f844-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6f844-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f844-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f844-116">Not supported.</span></span>|
|<span data-ttu-id="6f844-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6f844-117">Application</span></span>|<span data-ttu-id="6f844-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f844-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f844-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6f844-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="6f844-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f844-120">Request headers</span></span>
|<span data-ttu-id="6f844-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f844-121">Header</span></span>|<span data-ttu-id="6f844-122">値</span><span class="sxs-lookup"><span data-stu-id="6f844-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f844-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f844-123">Authorization</span></span>|<span data-ttu-id="6f844-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6f844-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f844-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f844-125">Accept</span></span>|<span data-ttu-id="6f844-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f844-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f844-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6f844-127">Request body</span></span>
<span data-ttu-id="6f844-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6f844-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f844-129">応答</span><span class="sxs-lookup"><span data-stu-id="6f844-129">Response</span></span>
<span data-ttu-id="6f844-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6f844-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f844-131">例</span><span class="sxs-lookup"><span data-stu-id="6f844-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f844-132">要求</span><span class="sxs-lookup"><span data-stu-id="6f844-132">Request</span></span>
<span data-ttu-id="6f844-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6f844-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="6f844-134">応答</span><span class="sxs-lookup"><span data-stu-id="6f844-134">Response</span></span>
<span data-ttu-id="6f844-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6f844-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1171

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBook",
      "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
      "largeCover": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "informationUrl": "https://example.com/informationUrl/",
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
      "appleId": "Apple Id value",
      "vppOrganizationName": "Vpp Organization Name value",
      "genres": [
        "Genres value"
      ],
      "language": "Language value",
      "seller": "Seller value",
      "totalLicenseCount": 1,
      "usedLicenseCount": 0,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




