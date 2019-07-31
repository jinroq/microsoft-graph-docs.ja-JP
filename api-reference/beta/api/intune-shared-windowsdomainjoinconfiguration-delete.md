---
title: WindowsDomainJoinConfiguration の削除
description: WindowsDomainJoinConfiguration を削除します。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af184a56a2391e8fb76cfa61ece292a9fa8af2f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979527"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="c18b3-103">WindowsDomainJoinConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="c18b3-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="c18b3-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="c18b3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c18b3-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c18b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c18b3-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c18b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c18b3-107">[Windowsdomainjoinconfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c18b3-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c18b3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c18b3-108">Prerequisites</span></span>
<span data-ttu-id="c18b3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c18b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c18b3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c18b3-111">Permission type</span></span>|<span data-ttu-id="c18b3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c18b3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c18b3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c18b3-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c18b3-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="c18b3-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="c18b3-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c18b3-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="c18b3-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c18b3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c18b3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c18b3-117">Not supported.</span></span>|
|<span data-ttu-id="c18b3-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c18b3-118">Application</span></span>|<span data-ttu-id="c18b3-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c18b3-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c18b3-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c18b3-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c18b3-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c18b3-121">Request headers</span></span>
|<span data-ttu-id="c18b3-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c18b3-122">Header</span></span>|<span data-ttu-id="c18b3-123">値</span><span class="sxs-lookup"><span data-stu-id="c18b3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c18b3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c18b3-124">Authorization</span></span>|<span data-ttu-id="c18b3-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c18b3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c18b3-126">承諾</span><span class="sxs-lookup"><span data-stu-id="c18b3-126">Accept</span></span>|<span data-ttu-id="c18b3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c18b3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c18b3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c18b3-128">Request body</span></span>
<span data-ttu-id="c18b3-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c18b3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c18b3-130">応答</span><span class="sxs-lookup"><span data-stu-id="c18b3-130">Response</span></span>
<span data-ttu-id="c18b3-131">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c18b3-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c18b3-132">例</span><span class="sxs-lookup"><span data-stu-id="c18b3-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="c18b3-133">要求</span><span class="sxs-lookup"><span data-stu-id="c18b3-133">Request</span></span>
<span data-ttu-id="c18b3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c18b3-134">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c18b3-135">応答</span><span class="sxs-lookup"><span data-stu-id="c18b3-135">Response</span></span>
<span data-ttu-id="c18b3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c18b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



