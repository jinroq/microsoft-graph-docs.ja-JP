---
title: deviceCategories のリスト
description: deviceCategory オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d25838240d55cf78bf2d36b4742c8d18a1cfb174
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025908"
---
# <a name="list-devicecategories"></a><span data-ttu-id="a1b28-103">deviceCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="a1b28-103">List deviceCategories</span></span>

> <span data-ttu-id="a1b28-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a1b28-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1b28-105">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a1b28-105">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1b28-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a1b28-106">Prerequisites</span></span>
<span data-ttu-id="a1b28-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1b28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1b28-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a1b28-109">Permission type</span></span>|<span data-ttu-id="a1b28-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a1b28-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1b28-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a1b28-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a1b28-112">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="a1b28-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="a1b28-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1b28-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="a1b28-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a1b28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1b28-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1b28-115">Not supported.</span></span>|
|<span data-ttu-id="a1b28-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a1b28-116">Application</span></span>|<span data-ttu-id="a1b28-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a1b28-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1b28-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a1b28-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="a1b28-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1b28-119">Request headers</span></span>
|<span data-ttu-id="a1b28-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a1b28-120">Header</span></span>|<span data-ttu-id="a1b28-121">値</span><span class="sxs-lookup"><span data-stu-id="a1b28-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1b28-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1b28-122">Authorization</span></span>|<span data-ttu-id="a1b28-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a1b28-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1b28-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a1b28-124">Accept</span></span>|<span data-ttu-id="a1b28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1b28-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1b28-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a1b28-126">Request body</span></span>
<span data-ttu-id="a1b28-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a1b28-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1b28-128">応答</span><span class="sxs-lookup"><span data-stu-id="a1b28-128">Response</span></span>
<span data-ttu-id="a1b28-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a1b28-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1b28-130">例</span><span class="sxs-lookup"><span data-stu-id="a1b28-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1b28-131">要求</span><span class="sxs-lookup"><span data-stu-id="a1b28-131">Request</span></span>
<span data-ttu-id="a1b28-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a1b28-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="a1b28-133">応答</span><span class="sxs-lookup"><span data-stu-id="a1b28-133">Response</span></span>
<span data-ttu-id="a1b28-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a1b28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCategory",
      "id": "f881b841-b841-f881-41b8-81f841b881f8",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```



