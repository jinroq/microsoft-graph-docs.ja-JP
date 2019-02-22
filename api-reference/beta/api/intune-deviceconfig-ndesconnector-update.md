---
title: ndesconnector の更新
description: ndesconnector オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4d51f22c71ef43784ec45e521f0e1900abdb9c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140279"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="a3364-103">ndesconnector の更新</span><span class="sxs-lookup"><span data-stu-id="a3364-103">Update ndesConnector</span></span>

> <span data-ttu-id="a3364-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3364-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3364-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3364-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3364-106">[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a3364-106">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3364-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a3364-107">Prerequisites</span></span>
<span data-ttu-id="a3364-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3364-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a3364-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3364-110">Permission type</span></span>|<span data-ttu-id="a3364-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3364-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3364-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3364-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3364-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3364-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3364-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3364-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3364-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3364-115">Not supported.</span></span>|
|<span data-ttu-id="a3364-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3364-116">Application</span></span>|<span data-ttu-id="a3364-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3364-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3364-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3364-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="a3364-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3364-119">Request headers</span></span>
|<span data-ttu-id="a3364-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3364-120">Header</span></span>|<span data-ttu-id="a3364-121">値</span><span class="sxs-lookup"><span data-stu-id="a3364-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3364-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3364-122">Authorization</span></span>|<span data-ttu-id="a3364-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a3364-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3364-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a3364-124">Accept</span></span>|<span data-ttu-id="a3364-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3364-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3364-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3364-126">Request body</span></span>
<span data-ttu-id="a3364-127">要求本文で、 [ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a3364-127">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="a3364-128">次の表に、 [ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a3364-128">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="a3364-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3364-129">Property</span></span>|<span data-ttu-id="a3364-130">型</span><span class="sxs-lookup"><span data-stu-id="a3364-130">Type</span></span>|<span data-ttu-id="a3364-131">説明</span><span class="sxs-lookup"><span data-stu-id="a3364-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3364-132">id</span><span class="sxs-lookup"><span data-stu-id="a3364-132">id</span></span>|<span data-ttu-id="a3364-133">String</span><span class="sxs-lookup"><span data-stu-id="a3364-133">String</span></span>|<span data-ttu-id="a3364-134">NDES connector のキー。</span><span class="sxs-lookup"><span data-stu-id="a3364-134">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="a3364-135">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="a3364-135">lastConnectionDateTime</span></span>|<span data-ttu-id="a3364-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3364-136">DateTimeOffset</span></span>|<span data-ttu-id="a3364-137">Ndes connector の最終接続時刻</span><span class="sxs-lookup"><span data-stu-id="a3364-137">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="a3364-138">state</span><span class="sxs-lookup"><span data-stu-id="a3364-138">state</span></span>|[<span data-ttu-id="a3364-139">ndesコネクタ状態</span><span class="sxs-lookup"><span data-stu-id="a3364-139">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="a3364-140">Ndes connector の状態。</span><span class="sxs-lookup"><span data-stu-id="a3364-140">Ndes Connector Status.</span></span> <span data-ttu-id="a3364-141">可能な値は `none`、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="a3364-141">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="a3364-142">displayName</span><span class="sxs-lookup"><span data-stu-id="a3364-142">displayName</span></span>|<span data-ttu-id="a3364-143">String</span><span class="sxs-lookup"><span data-stu-id="a3364-143">String</span></span>|<span data-ttu-id="a3364-144">Ndes connector のフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="a3364-144">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="a3364-145">応答</span><span class="sxs-lookup"><span data-stu-id="a3364-145">Response</span></span>
<span data-ttu-id="a3364-146">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a3364-146">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3364-147">例</span><span class="sxs-lookup"><span data-stu-id="a3364-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3364-148">要求</span><span class="sxs-lookup"><span data-stu-id="a3364-148">Request</span></span>
<span data-ttu-id="a3364-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a3364-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="a3364-150">応答</span><span class="sxs-lookup"><span data-stu-id="a3364-150">Response</span></span>
<span data-ttu-id="a3364-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a3364-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```




