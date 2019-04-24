---
title: ndesconnector の作成
description: 新しい ndesconnector オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8c105758f5d65e64c90a9928732c78ec8bb4f2e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518164"
---
# <a name="create-ndesconnector"></a><span data-ttu-id="4c6c4-103">ndesconnector の作成</span><span class="sxs-lookup"><span data-stu-id="4c6c4-103">Create ndesConnector</span></span>

> <span data-ttu-id="4c6c4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c6c4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c6c4-106">新しい[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-106">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c6c4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4c6c4-107">Prerequisites</span></span>
<span data-ttu-id="4c6c4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c6c4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c6c4-110">Permission type</span></span>|<span data-ttu-id="4c6c4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c6c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c6c4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c6c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c6c4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c6c4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c6c4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c6c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c6c4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-115">Not supported.</span></span>|
|<span data-ttu-id="4c6c4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c6c4-116">Application</span></span>|<span data-ttu-id="4c6c4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c6c4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c6c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="4c6c4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c6c4-119">Request headers</span></span>
|<span data-ttu-id="4c6c4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c6c4-120">Header</span></span>|<span data-ttu-id="4c6c4-121">値</span><span class="sxs-lookup"><span data-stu-id="4c6c4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c6c4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c6c4-122">Authorization</span></span>|<span data-ttu-id="4c6c4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c6c4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4c6c4-124">Accept</span></span>|<span data-ttu-id="4c6c4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c6c4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c6c4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c6c4-126">Request body</span></span>
<span data-ttu-id="4c6c4-127">要求本文で、ndesconnector オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-127">In the request body, supply a JSON representation for the ndesConnector object.</span></span>

<span data-ttu-id="4c6c4-128">次の表に、ndesconnector の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-128">The following table shows the properties that are required when you create the ndesConnector.</span></span>

|<span data-ttu-id="4c6c4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c6c4-129">Property</span></span>|<span data-ttu-id="4c6c4-130">型</span><span class="sxs-lookup"><span data-stu-id="4c6c4-130">Type</span></span>|<span data-ttu-id="4c6c4-131">説明</span><span class="sxs-lookup"><span data-stu-id="4c6c4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c6c4-132">id</span><span class="sxs-lookup"><span data-stu-id="4c6c4-132">id</span></span>|<span data-ttu-id="4c6c4-133">String</span><span class="sxs-lookup"><span data-stu-id="4c6c4-133">String</span></span>|<span data-ttu-id="4c6c4-134">NDES connector のキー。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-134">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="4c6c4-135">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="4c6c4-135">lastConnectionDateTime</span></span>|<span data-ttu-id="4c6c4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c6c4-136">DateTimeOffset</span></span>|<span data-ttu-id="4c6c4-137">Ndes connector の最終接続時刻</span><span class="sxs-lookup"><span data-stu-id="4c6c4-137">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="4c6c4-138">state</span><span class="sxs-lookup"><span data-stu-id="4c6c4-138">state</span></span>|[<span data-ttu-id="4c6c4-139">ndesコネクタ状態</span><span class="sxs-lookup"><span data-stu-id="4c6c4-139">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="4c6c4-140">Ndes connector の状態。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-140">Ndes Connector Status.</span></span> <span data-ttu-id="4c6c4-141">使用可能な値は、`none`、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-141">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="4c6c4-142">displayName</span><span class="sxs-lookup"><span data-stu-id="4c6c4-142">displayName</span></span>|<span data-ttu-id="4c6c4-143">String</span><span class="sxs-lookup"><span data-stu-id="4c6c4-143">String</span></span>|<span data-ttu-id="4c6c4-144">Ndes connector のフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-144">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="4c6c4-145">応答</span><span class="sxs-lookup"><span data-stu-id="4c6c4-145">Response</span></span>
<span data-ttu-id="4c6c4-146">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-146">If successful, this method returns a `201 Created` response code and a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c6c4-147">例</span><span class="sxs-lookup"><span data-stu-id="4c6c4-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c6c4-148">要求</span><span class="sxs-lookup"><span data-stu-id="4c6c4-148">Request</span></span>
<span data-ttu-id="4c6c4-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c6c4-150">応答</span><span class="sxs-lookup"><span data-stu-id="4c6c4-150">Response</span></span>
<span data-ttu-id="4c6c4-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c6c4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





