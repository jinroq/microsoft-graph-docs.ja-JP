---
title: managedEBooks のリスト
description: managedEBook オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88e7c4a76bd8a0d9856a49f7d14169c6e27f5be4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979299"
---
# <a name="list-managedebooks"></a><span data-ttu-id="04844-103">managedEBooks のリスト</span><span class="sxs-lookup"><span data-stu-id="04844-103">List managedEBooks</span></span>

> <span data-ttu-id="04844-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="04844-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04844-105">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="04844-105">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04844-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="04844-106">Prerequisites</span></span>
<span data-ttu-id="04844-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04844-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04844-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04844-109">Permission type</span></span>|<span data-ttu-id="04844-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="04844-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04844-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04844-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04844-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="04844-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="04844-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04844-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04844-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04844-114">Not supported.</span></span>|
|<span data-ttu-id="04844-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04844-115">Application</span></span>|<span data-ttu-id="04844-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04844-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04844-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04844-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="04844-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04844-118">Request headers</span></span>
|<span data-ttu-id="04844-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04844-119">Header</span></span>|<span data-ttu-id="04844-120">値</span><span class="sxs-lookup"><span data-stu-id="04844-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04844-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="04844-121">Authorization</span></span>|<span data-ttu-id="04844-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="04844-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04844-123">承諾</span><span class="sxs-lookup"><span data-stu-id="04844-123">Accept</span></span>|<span data-ttu-id="04844-124">application/json</span><span class="sxs-lookup"><span data-stu-id="04844-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04844-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="04844-125">Request body</span></span>
<span data-ttu-id="04844-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="04844-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04844-127">応答</span><span class="sxs-lookup"><span data-stu-id="04844-127">Response</span></span>
<span data-ttu-id="04844-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedEBook](../resources/intune-books-managedebook.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="04844-128">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04844-129">例</span><span class="sxs-lookup"><span data-stu-id="04844-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="04844-130">要求</span><span class="sxs-lookup"><span data-stu-id="04844-130">Request</span></span>
<span data-ttu-id="04844-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04844-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="04844-132">応答</span><span class="sxs-lookup"><span data-stu-id="04844-132">Response</span></span>
<span data-ttu-id="04844-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04844-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBook",
      "id": "1fbd3558-3558-1fbd-5835-bd1f5835bd1f",
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
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
    }
  ]
}
```



