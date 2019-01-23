---
title: NdesConnector を作成します。
description: 新しい ndesConnector オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2764e461b0cfce3e620c5e5300539297b9cb5b1f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419934"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="3d4c6-103">NdesConnector を作成します。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-103">Create ndesConnector</span></span>

> <span data-ttu-id="3d4c6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3d4c6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3d4c6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d4c6-107">新しい[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-107">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d4c6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3d4c6-108">Prerequisites</span></span>
<span data-ttu-id="3d4c6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3d4c6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3d4c6-111">Permission type</span></span>|<span data-ttu-id="3d4c6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3d4c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d4c6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3d4c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d4c6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d4c6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3d4c6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3d4c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d4c6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-116">Not supported.</span></span>|
|<span data-ttu-id="3d4c6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3d4c6-117">Application</span></span>|<span data-ttu-id="3d4c6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d4c6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d4c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="3d4c6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d4c6-120">Request headers</span></span>
|<span data-ttu-id="3d4c6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d4c6-121">Header</span></span>|<span data-ttu-id="3d4c6-122">値</span><span class="sxs-lookup"><span data-stu-id="3d4c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d4c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d4c6-123">Authorization</span></span>|<span data-ttu-id="3d4c6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d4c6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d4c6-125">Accept</span></span>|<span data-ttu-id="3d4c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d4c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d4c6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d4c6-127">Request body</span></span>
<span data-ttu-id="3d4c6-128">要求の本文に ndesConnector オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-128">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="3d4c6-129">次の表は、ndesConnector を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-129">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="3d4c6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3d4c6-130">Property</span></span>|<span data-ttu-id="3d4c6-131">型</span><span class="sxs-lookup"><span data-stu-id="3d4c6-131">Type</span></span>|<span data-ttu-id="3d4c6-132">説明</span><span class="sxs-lookup"><span data-stu-id="3d4c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d4c6-133">id</span><span class="sxs-lookup"><span data-stu-id="3d4c6-133">id</span></span>|<span data-ttu-id="3d4c6-134">String</span><span class="sxs-lookup"><span data-stu-id="3d4c6-134">String</span></span>|<span data-ttu-id="3d4c6-135">NDES のコネクタのキー。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="3d4c6-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="3d4c6-136">lastConnectionDateTime</span></span>|<span data-ttu-id="3d4c6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d4c6-137">DateTimeOffset</span></span>|<span data-ttu-id="3d4c6-138">Ndes コネクタの前回の接続</span><span class="sxs-lookup"><span data-stu-id="3d4c6-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="3d4c6-139">state</span><span class="sxs-lookup"><span data-stu-id="3d4c6-139">state</span></span>|[<span data-ttu-id="3d4c6-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="3d4c6-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="3d4c6-141">Ndes のコネクタの状態です。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-141">Ndes Connector Status.</span></span> <span data-ttu-id="3d4c6-142">可能な値は、`none`、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="3d4c6-143">displayName</span><span class="sxs-lookup"><span data-stu-id="3d4c6-143">displayName</span></span>|<span data-ttu-id="3d4c6-144">String</span><span class="sxs-lookup"><span data-stu-id="3d4c6-144">String</span></span>|<span data-ttu-id="3d4c6-145">Ndes のコネクタの表示名。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="3d4c6-146">応答</span><span class="sxs-lookup"><span data-stu-id="3d4c6-146">Response</span></span>
<span data-ttu-id="3d4c6-147">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-147">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d4c6-148">例</span><span class="sxs-lookup"><span data-stu-id="3d4c6-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d4c6-149">要求</span><span class="sxs-lookup"><span data-stu-id="3d4c6-149">Request</span></span>
<span data-ttu-id="3d4c6-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="3d4c6-151">応答</span><span class="sxs-lookup"><span data-stu-id="3d4c6-151">Response</span></span>
<span data-ttu-id="3d4c6-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3d4c6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




