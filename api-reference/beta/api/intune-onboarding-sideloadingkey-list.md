---
title: リスト sideLoadingKeies
description: SideLoadingKey オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b18da0d1d5c5da63007f489708938cefb9dd51f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352408"
---
# <a name="list-sideloadingkeies"></a><span data-ttu-id="85107-103">リスト sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="85107-103">List sideLoadingKeies</span></span>

> <span data-ttu-id="85107-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85107-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85107-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="85107-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85107-106">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="85107-106">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85107-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="85107-107">Prerequisites</span></span>
<span data-ttu-id="85107-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85107-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85107-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85107-110">Permission type</span></span>|<span data-ttu-id="85107-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="85107-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85107-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85107-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85107-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="85107-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="85107-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85107-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85107-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85107-115">Not supported.</span></span>|
|<span data-ttu-id="85107-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85107-116">Application</span></span>|<span data-ttu-id="85107-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="85107-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85107-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85107-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="85107-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85107-119">Request headers</span></span>
|<span data-ttu-id="85107-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85107-120">Header</span></span>|<span data-ttu-id="85107-121">値</span><span class="sxs-lookup"><span data-stu-id="85107-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85107-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85107-122">Authorization</span></span>|<span data-ttu-id="85107-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="85107-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85107-124">承諾</span><span class="sxs-lookup"><span data-stu-id="85107-124">Accept</span></span>|<span data-ttu-id="85107-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85107-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85107-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="85107-126">Request body</span></span>
<span data-ttu-id="85107-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="85107-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85107-128">応答</span><span class="sxs-lookup"><span data-stu-id="85107-128">Response</span></span>
<span data-ttu-id="85107-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="85107-129">If successful, this method returns a `200 OK` response code and a collection of [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85107-130">例</span><span class="sxs-lookup"><span data-stu-id="85107-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="85107-131">要求</span><span class="sxs-lookup"><span data-stu-id="85107-131">Request</span></span>
<span data-ttu-id="85107-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="85107-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
```

### <a name="response"></a><span data-ttu-id="85107-133">応答</span><span class="sxs-lookup"><span data-stu-id="85107-133">Response</span></span>
<span data-ttu-id="85107-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="85107-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sideLoadingKey",
      "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
      "value": "Value value",
      "displayName": "Display Name value",
      "description": "Description value",
      "totalActivation": 15,
      "lastUpdatedDateTime": "Last Updated Date Time value"
    }
  ]
}
```






