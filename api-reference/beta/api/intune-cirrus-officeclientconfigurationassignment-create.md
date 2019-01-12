---
title: OfficeClientConfigurationAssignment を作成します。
description: ターゲット グループを既存のポリシーに追加します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20ce558795abcf35cdcaad8386d1b875a2bf3f81
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954275"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="924d2-103">OfficeClientConfigurationAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="924d2-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="924d2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="924d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="924d2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="924d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="924d2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="924d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="924d2-107">ターゲット グループを既存のポリシーに追加します。</span><span class="sxs-lookup"><span data-stu-id="924d2-107">Add a target group to an existing policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="924d2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="924d2-108">Prerequisites</span></span>
<span data-ttu-id="924d2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="924d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="924d2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="924d2-111">Permission type</span></span>|<span data-ttu-id="924d2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="924d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="924d2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="924d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="924d2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="924d2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="924d2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="924d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="924d2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="924d2-116">Not supported.</span></span>|
|<span data-ttu-id="924d2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="924d2-117">Application</span></span>|<span data-ttu-id="924d2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="924d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="924d2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="924d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="924d2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="924d2-120">Request headers</span></span>
|<span data-ttu-id="924d2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="924d2-121">Header</span></span>|<span data-ttu-id="924d2-122">値</span><span class="sxs-lookup"><span data-stu-id="924d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="924d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="924d2-123">Authorization</span></span>|<span data-ttu-id="924d2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="924d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="924d2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="924d2-125">Accept</span></span>|<span data-ttu-id="924d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="924d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="924d2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="924d2-127">Request body</span></span>
<span data-ttu-id="924d2-128">要求の本文に officeClientConfigurationAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="924d2-128">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="924d2-129">次の表は、officeClientConfigurationAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="924d2-129">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="924d2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="924d2-130">Property</span></span>|<span data-ttu-id="924d2-131">型</span><span class="sxs-lookup"><span data-stu-id="924d2-131">Type</span></span>|<span data-ttu-id="924d2-132">説明</span><span class="sxs-lookup"><span data-stu-id="924d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="924d2-133">ID</span><span class="sxs-lookup"><span data-stu-id="924d2-133">id</span></span>|<span data-ttu-id="924d2-134">String</span><span class="sxs-lookup"><span data-stu-id="924d2-134">String</span></span>|<span data-ttu-id="924d2-135">OfficeConfigurationAssignment の id です。</span><span class="sxs-lookup"><span data-stu-id="924d2-135">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="924d2-136">ターゲット</span><span class="sxs-lookup"><span data-stu-id="924d2-136">target</span></span>|[<span data-ttu-id="924d2-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="924d2-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="924d2-138">Admin によって定義されているターゲットの割り当て</span><span class="sxs-lookup"><span data-stu-id="924d2-138">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="924d2-139">応答</span><span class="sxs-lookup"><span data-stu-id="924d2-139">Response</span></span>
<span data-ttu-id="924d2-140">かどうかは成功すると、このメソッドが返されます、`200 Created`応答コードおよび応答の本文に[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="924d2-140">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="924d2-141">例</span><span class="sxs-lookup"><span data-stu-id="924d2-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="924d2-142">要求</span><span class="sxs-lookup"><span data-stu-id="924d2-142">Request</span></span>
<span data-ttu-id="924d2-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="924d2-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="924d2-144">応答</span><span class="sxs-lookup"><span data-stu-id="924d2-144">Response</span></span>
<span data-ttu-id="924d2-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="924d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



