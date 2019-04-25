---
title: Get deviceConfigurationAssignment
description: deviceConfigurationAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97e6b932ce96246d127c16a75b6ffae78a21daa1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575318"
---
# <a name="get-deviceconfigurationassignment"></a><span data-ttu-id="6cb6f-103">Get deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6cb6f-103">Get deviceConfigurationAssignment</span></span>

> <span data-ttu-id="6cb6f-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6cb6f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cb6f-105">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6cb6f-105">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cb6f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6cb6f-106">Prerequisites</span></span>
<span data-ttu-id="6cb6f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6cb6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cb6f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6cb6f-109">Permission type</span></span>|<span data-ttu-id="6cb6f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6cb6f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cb6f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6cb6f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6cb6f-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6cb6f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6cb6f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6cb6f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cb6f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cb6f-114">Not supported.</span></span>|
|<span data-ttu-id="6cb6f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6cb6f-115">Application</span></span>|<span data-ttu-id="6cb6f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cb6f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cb6f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6cb6f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6cb6f-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6cb6f-118">Optional query parameters</span></span>
<span data-ttu-id="6cb6f-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6cb6f-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6cb6f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cb6f-120">Request headers</span></span>
|<span data-ttu-id="6cb6f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6cb6f-121">Header</span></span>|<span data-ttu-id="6cb6f-122">値</span><span class="sxs-lookup"><span data-stu-id="6cb6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cb6f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cb6f-123">Authorization</span></span>|<span data-ttu-id="6cb6f-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6cb6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cb6f-125">承諾</span><span class="sxs-lookup"><span data-stu-id="6cb6f-125">Accept</span></span>|<span data-ttu-id="6cb6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cb6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cb6f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6cb6f-127">Request body</span></span>
<span data-ttu-id="6cb6f-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6cb6f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6cb6f-129">応答</span><span class="sxs-lookup"><span data-stu-id="6cb6f-129">Response</span></span>
<span data-ttu-id="6cb6f-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6cb6f-130">If successful, this method returns a `200 OK` response code and [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cb6f-131">例</span><span class="sxs-lookup"><span data-stu-id="6cb6f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cb6f-132">要求</span><span class="sxs-lookup"><span data-stu-id="6cb6f-132">Request</span></span>
<span data-ttu-id="6cb6f-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6cb6f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="6cb6f-134">応答</span><span class="sxs-lookup"><span data-stu-id="6cb6f-134">Response</span></span>
<span data-ttu-id="6cb6f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6cb6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
    "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



