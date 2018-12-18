---
title: NdesConnector を作成します。
description: 新しい ndesConnector オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 16580e9d69850139edd8f268bbaf3688b29d06e7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333601"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="d874b-103">NdesConnector を作成します。</span><span class="sxs-lookup"><span data-stu-id="d874b-103">Create ndesConnector</span></span>

> <span data-ttu-id="d874b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d874b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d874b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d874b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d874b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d874b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d874b-107">新しい[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d874b-107">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d874b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d874b-108">Prerequisites</span></span>
<span data-ttu-id="d874b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d874b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d874b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d874b-111">Permission type</span></span>|<span data-ttu-id="d874b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d874b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d874b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d874b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d874b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d874b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d874b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d874b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d874b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d874b-116">Not supported.</span></span>|
|<span data-ttu-id="d874b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d874b-117">Application</span></span>|<span data-ttu-id="d874b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d874b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d874b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d874b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="d874b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d874b-120">Request headers</span></span>
|<span data-ttu-id="d874b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d874b-121">Header</span></span>|<span data-ttu-id="d874b-122">値</span><span class="sxs-lookup"><span data-stu-id="d874b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d874b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d874b-123">Authorization</span></span>|<span data-ttu-id="d874b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d874b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d874b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d874b-125">Accept</span></span>|<span data-ttu-id="d874b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d874b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d874b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d874b-127">Request body</span></span>
<span data-ttu-id="d874b-128">要求の本文に ndesConnector オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d874b-128">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="d874b-129">次の表は、ndesConnector を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d874b-129">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="d874b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d874b-130">Property</span></span>|<span data-ttu-id="d874b-131">種類</span><span class="sxs-lookup"><span data-stu-id="d874b-131">Type</span></span>|<span data-ttu-id="d874b-132">説明</span><span class="sxs-lookup"><span data-stu-id="d874b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d874b-133">ID</span><span class="sxs-lookup"><span data-stu-id="d874b-133">id</span></span>|<span data-ttu-id="d874b-134">String</span><span class="sxs-lookup"><span data-stu-id="d874b-134">String</span></span>|<span data-ttu-id="d874b-135">NDES のコネクタのキー。</span><span class="sxs-lookup"><span data-stu-id="d874b-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="d874b-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="d874b-136">lastConnectionDateTime</span></span>|<span data-ttu-id="d874b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d874b-137">DateTimeOffset</span></span>|<span data-ttu-id="d874b-138">Ndes コネクタの前回の接続</span><span class="sxs-lookup"><span data-stu-id="d874b-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="d874b-139">state</span><span class="sxs-lookup"><span data-stu-id="d874b-139">state</span></span>|[<span data-ttu-id="d874b-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="d874b-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="d874b-141">Ndes のコネクタの状態です。</span><span class="sxs-lookup"><span data-stu-id="d874b-141">Ndes Connector Status.</span></span> <span data-ttu-id="d874b-142">可能な値は、`none`、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="d874b-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="d874b-143">displayName</span><span class="sxs-lookup"><span data-stu-id="d874b-143">displayName</span></span>|<span data-ttu-id="d874b-144">String</span><span class="sxs-lookup"><span data-stu-id="d874b-144">String</span></span>|<span data-ttu-id="d874b-145">Ndes のコネクタの表示名。</span><span class="sxs-lookup"><span data-stu-id="d874b-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="d874b-146">応答</span><span class="sxs-lookup"><span data-stu-id="d874b-146">Response</span></span>
<span data-ttu-id="d874b-147">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d874b-147">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d874b-148">例</span><span class="sxs-lookup"><span data-stu-id="d874b-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="d874b-149">要求</span><span class="sxs-lookup"><span data-stu-id="d874b-149">Request</span></span>
<span data-ttu-id="d874b-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d874b-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d874b-151">応答</span><span class="sxs-lookup"><span data-stu-id="d874b-151">Response</span></span>
<span data-ttu-id="d874b-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d874b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





