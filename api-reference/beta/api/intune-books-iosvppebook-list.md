---
title: iosVppEBooks のリスト
description: iosVppEBook オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ee90d7551939ddcb74a8c0e6120c1c7801ff08f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972376"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="606ce-103">iosVppEBooks のリスト</span><span class="sxs-lookup"><span data-stu-id="606ce-103">List iosVppEBooks</span></span>

> <span data-ttu-id="606ce-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="606ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="606ce-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="606ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="606ce-106">[iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="606ce-106">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="606ce-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="606ce-107">Prerequisites</span></span>
<span data-ttu-id="606ce-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="606ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="606ce-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="606ce-110">Permission type</span></span>|<span data-ttu-id="606ce-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="606ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="606ce-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="606ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="606ce-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="606ce-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="606ce-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="606ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="606ce-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="606ce-115">Not supported.</span></span>|
|<span data-ttu-id="606ce-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="606ce-116">Application</span></span>|<span data-ttu-id="606ce-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="606ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="606ce-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="606ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="606ce-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="606ce-119">Request headers</span></span>
|<span data-ttu-id="606ce-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="606ce-120">Header</span></span>|<span data-ttu-id="606ce-121">値</span><span class="sxs-lookup"><span data-stu-id="606ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="606ce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="606ce-122">Authorization</span></span>|<span data-ttu-id="606ce-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="606ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="606ce-124">承諾</span><span class="sxs-lookup"><span data-stu-id="606ce-124">Accept</span></span>|<span data-ttu-id="606ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="606ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="606ce-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="606ce-126">Request body</span></span>
<span data-ttu-id="606ce-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="606ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="606ce-128">応答</span><span class="sxs-lookup"><span data-stu-id="606ce-128">Response</span></span>
<span data-ttu-id="606ce-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="606ce-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="606ce-130">例</span><span class="sxs-lookup"><span data-stu-id="606ce-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="606ce-131">要求</span><span class="sxs-lookup"><span data-stu-id="606ce-131">Request</span></span>
<span data-ttu-id="606ce-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="606ce-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="606ce-133">応答</span><span class="sxs-lookup"><span data-stu-id="606ce-133">Response</span></span>
<span data-ttu-id="606ce-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="606ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





