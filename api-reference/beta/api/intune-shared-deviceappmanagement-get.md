---
title: Get deviceAppManagement
description: deviceAppManagement オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f7bfd02d2e98386fa8f9e6172cfdfcfeb63af5b4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989547"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="23e36-103">Get deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="23e36-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="23e36-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="23e36-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="23e36-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23e36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23e36-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="23e36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23e36-107">[deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="23e36-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23e36-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="23e36-108">Prerequisites</span></span>

<span data-ttu-id="23e36-109">この API を呼び出すには、次のいずれかのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="23e36-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="23e36-110">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23e36-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="23e36-111">適切なアクセス許可は、ワークフローによって異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="23e36-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="23e36-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="23e36-112">Permission type</span></span>|<span data-ttu-id="23e36-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="23e36-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="23e36-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="23e36-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="23e36-115">&nbsp;&nbsp; **アプリ**、**ブック**、**オンボード**、または**パートナーの統合**</span><span class="sxs-lookup"><span data-stu-id="23e36-115">&nbsp; &nbsp; **Apps**, **books**, **onboarding**, or **Partner Integration**</span></span> | <span data-ttu-id="23e36-116">Devicemanagementapps の、DeviceManagementApps. ReadW すべて</span><span class="sxs-lookup"><span data-stu-id="23e36-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="23e36-117">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="23e36-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="23e36-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="23e36-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="23e36-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="23e36-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23e36-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23e36-120">Not supported.</span></span>|
|<span data-ttu-id="23e36-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="23e36-121">Application</span></span>|<span data-ttu-id="23e36-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23e36-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23e36-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="23e36-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23e36-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="23e36-124">Optional query parameters</span></span>

<span data-ttu-id="23e36-125">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="23e36-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23e36-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23e36-126">Request headers</span></span>

|<span data-ttu-id="23e36-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23e36-127">Header</span></span>|<span data-ttu-id="23e36-128">値</span><span class="sxs-lookup"><span data-stu-id="23e36-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23e36-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="23e36-129">Authorization</span></span>|<span data-ttu-id="23e36-130">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="23e36-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23e36-131">承諾</span><span class="sxs-lookup"><span data-stu-id="23e36-131">Accept</span></span>|<span data-ttu-id="23e36-132">application/json</span><span class="sxs-lookup"><span data-stu-id="23e36-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23e36-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="23e36-133">Request body</span></span>

<span data-ttu-id="23e36-134">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="23e36-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23e36-135">応答</span><span class="sxs-lookup"><span data-stu-id="23e36-135">Response</span></span>

<span data-ttu-id="23e36-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="23e36-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23e36-137">例</span><span class="sxs-lookup"><span data-stu-id="23e36-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="23e36-138">要求</span><span class="sxs-lookup"><span data-stu-id="23e36-138">Request</span></span>

<span data-ttu-id="23e36-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="23e36-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="23e36-140">応答</span><span class="sxs-lookup"><span data-stu-id="23e36-140">Response</span></span>

<span data-ttu-id="23e36-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="23e36-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



