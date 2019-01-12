---
title: NdesConnector を作成します。
description: 新しい ndesConnector オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 809a324665136927796790e88d3beb742cf06be4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940184"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="16317-103">NdesConnector を作成します。</span><span class="sxs-lookup"><span data-stu-id="16317-103">Create ndesConnector</span></span>

> <span data-ttu-id="16317-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16317-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16317-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16317-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16317-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="16317-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16317-107">新しい[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="16317-107">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16317-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="16317-108">Prerequisites</span></span>
<span data-ttu-id="16317-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16317-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16317-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16317-111">Permission type</span></span>|<span data-ttu-id="16317-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="16317-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16317-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16317-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16317-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16317-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16317-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16317-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16317-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16317-116">Not supported.</span></span>|
|<span data-ttu-id="16317-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16317-117">Application</span></span>|<span data-ttu-id="16317-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16317-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16317-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16317-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="16317-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16317-120">Request headers</span></span>
|<span data-ttu-id="16317-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16317-121">Header</span></span>|<span data-ttu-id="16317-122">値</span><span class="sxs-lookup"><span data-stu-id="16317-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16317-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16317-123">Authorization</span></span>|<span data-ttu-id="16317-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="16317-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16317-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16317-125">Accept</span></span>|<span data-ttu-id="16317-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16317-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16317-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="16317-127">Request body</span></span>
<span data-ttu-id="16317-128">要求の本文に ndesConnector オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="16317-128">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="16317-129">次の表は、ndesConnector を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="16317-129">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="16317-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16317-130">Property</span></span>|<span data-ttu-id="16317-131">種類</span><span class="sxs-lookup"><span data-stu-id="16317-131">Type</span></span>|<span data-ttu-id="16317-132">説明</span><span class="sxs-lookup"><span data-stu-id="16317-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16317-133">ID</span><span class="sxs-lookup"><span data-stu-id="16317-133">id</span></span>|<span data-ttu-id="16317-134">String</span><span class="sxs-lookup"><span data-stu-id="16317-134">String</span></span>|<span data-ttu-id="16317-135">NDES のコネクタのキー。</span><span class="sxs-lookup"><span data-stu-id="16317-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="16317-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="16317-136">lastConnectionDateTime</span></span>|<span data-ttu-id="16317-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16317-137">DateTimeOffset</span></span>|<span data-ttu-id="16317-138">Ndes コネクタの前回の接続</span><span class="sxs-lookup"><span data-stu-id="16317-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="16317-139">state</span><span class="sxs-lookup"><span data-stu-id="16317-139">state</span></span>|[<span data-ttu-id="16317-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="16317-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="16317-141">Ndes のコネクタの状態です。</span><span class="sxs-lookup"><span data-stu-id="16317-141">Ndes Connector Status.</span></span> <span data-ttu-id="16317-142">可能な値は、`none`、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="16317-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="16317-143">displayName</span><span class="sxs-lookup"><span data-stu-id="16317-143">displayName</span></span>|<span data-ttu-id="16317-144">String</span><span class="sxs-lookup"><span data-stu-id="16317-144">String</span></span>|<span data-ttu-id="16317-145">Ndes のコネクタの表示名。</span><span class="sxs-lookup"><span data-stu-id="16317-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="16317-146">応答</span><span class="sxs-lookup"><span data-stu-id="16317-146">Response</span></span>
<span data-ttu-id="16317-147">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="16317-147">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16317-148">例</span><span class="sxs-lookup"><span data-stu-id="16317-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="16317-149">要求</span><span class="sxs-lookup"><span data-stu-id="16317-149">Request</span></span>
<span data-ttu-id="16317-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16317-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16317-151">応答</span><span class="sxs-lookup"><span data-stu-id="16317-151">Response</span></span>
<span data-ttu-id="16317-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="16317-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





