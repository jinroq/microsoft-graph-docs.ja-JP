---
title: iosCertificateProfiles のリスト
description: iosCertificateProfile オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69eb37955705cfb808570e3ca039754d00a0a363
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551485"
---
# <a name="list-ioscertificateprofiles"></a><span data-ttu-id="bc8cb-103">iosCertificateProfiles のリスト</span><span class="sxs-lookup"><span data-stu-id="bc8cb-103">List iosCertificateProfiles</span></span>

> <span data-ttu-id="bc8cb-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc8cb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc8cb-105">[iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bc8cb-105">List properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc8cb-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="bc8cb-106">Prerequisites</span></span>
<span data-ttu-id="bc8cb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc8cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc8cb-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bc8cb-109">Permission type</span></span>|<span data-ttu-id="bc8cb-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bc8cb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc8cb-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bc8cb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bc8cb-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc8cb-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bc8cb-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bc8cb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc8cb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc8cb-114">Not supported.</span></span>|
|<span data-ttu-id="bc8cb-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc8cb-115">Application</span></span>|<span data-ttu-id="bc8cb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc8cb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc8cb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bc8cb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bc8cb-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc8cb-118">Request headers</span></span>
|<span data-ttu-id="bc8cb-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc8cb-119">Header</span></span>|<span data-ttu-id="bc8cb-120">値</span><span class="sxs-lookup"><span data-stu-id="bc8cb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc8cb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc8cb-121">Authorization</span></span>|<span data-ttu-id="bc8cb-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc8cb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc8cb-123">承諾</span><span class="sxs-lookup"><span data-stu-id="bc8cb-123">Accept</span></span>|<span data-ttu-id="bc8cb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bc8cb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc8cb-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bc8cb-125">Request body</span></span>
<span data-ttu-id="bc8cb-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bc8cb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc8cb-127">応答</span><span class="sxs-lookup"><span data-stu-id="bc8cb-127">Response</span></span>
<span data-ttu-id="bc8cb-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bc8cb-128">If successful, this method returns a `200 OK` response code and a collection of [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc8cb-129">例</span><span class="sxs-lookup"><span data-stu-id="bc8cb-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc8cb-130">要求</span><span class="sxs-lookup"><span data-stu-id="bc8cb-130">Request</span></span>
<span data-ttu-id="bc8cb-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bc8cb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="bc8cb-132">応答</span><span class="sxs-lookup"><span data-stu-id="bc8cb-132">Response</span></span>
<span data-ttu-id="bc8cb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bc8cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCertificateProfile",
      "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```



