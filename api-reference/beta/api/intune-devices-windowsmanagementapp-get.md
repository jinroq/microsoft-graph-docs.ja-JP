---
title: windowsmanagementapp の取得
description: windowsmanagementapp オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b4c2255c1489ae969f9f5f0ddf35cdb644723e5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784657"
---
# <a name="get-windowsmanagementapp"></a><span data-ttu-id="196ca-103">windowsmanagementapp の取得</span><span class="sxs-lookup"><span data-stu-id="196ca-103">Get windowsManagementApp</span></span>

> <span data-ttu-id="196ca-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="196ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="196ca-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="196ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="196ca-106">[windowsmanagementapp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="196ca-106">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="196ca-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="196ca-107">Prerequisites</span></span>
<span data-ttu-id="196ca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="196ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="196ca-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="196ca-110">Permission type</span></span>|<span data-ttu-id="196ca-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="196ca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="196ca-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="196ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="196ca-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="196ca-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="196ca-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="196ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="196ca-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="196ca-115">Not supported.</span></span>|
|<span data-ttu-id="196ca-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="196ca-116">Application</span></span>|<span data-ttu-id="196ca-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="196ca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="196ca-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="196ca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp
```

## <a name="optional-query-parameters"></a><span data-ttu-id="196ca-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="196ca-119">Optional query parameters</span></span>
<span data-ttu-id="196ca-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="196ca-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="196ca-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="196ca-121">Request headers</span></span>
|<span data-ttu-id="196ca-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="196ca-122">Header</span></span>|<span data-ttu-id="196ca-123">値</span><span class="sxs-lookup"><span data-stu-id="196ca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="196ca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="196ca-124">Authorization</span></span>|<span data-ttu-id="196ca-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="196ca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="196ca-126">承諾</span><span class="sxs-lookup"><span data-stu-id="196ca-126">Accept</span></span>|<span data-ttu-id="196ca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="196ca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="196ca-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="196ca-128">Request body</span></span>
<span data-ttu-id="196ca-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="196ca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="196ca-130">応答</span><span class="sxs-lookup"><span data-stu-id="196ca-130">Response</span></span>
<span data-ttu-id="196ca-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowsmanagementapp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="196ca-131">If successful, this method returns a `200 OK` response code and [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="196ca-132">例</span><span class="sxs-lookup"><span data-stu-id="196ca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="196ca-133">要求</span><span class="sxs-lookup"><span data-stu-id="196ca-133">Request</span></span>
<span data-ttu-id="196ca-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="196ca-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
```

### <a name="response"></a><span data-ttu-id="196ca-135">応答</span><span class="sxs-lookup"><span data-stu-id="196ca-135">Response</span></span>
<span data-ttu-id="196ca-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="196ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsManagementApp",
    "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
    "availableVersion": "Available Version value"
  }
}
```





