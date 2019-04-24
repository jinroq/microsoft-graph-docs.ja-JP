---
title: Delete roleDefinition
description: roleDefinition を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f9bfafede8ef650b7f961ed45ec70ee4febadda3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585332"
---
# <a name="delete-roledefinition"></a><span data-ttu-id="eddfe-103">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="eddfe-103">Delete roleDefinition</span></span>

> <span data-ttu-id="eddfe-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eddfe-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eddfe-105">[roleDefinition](../resources/intune-rbac-roledefinition.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="eddfe-105">Deletes a [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eddfe-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="eddfe-106">Prerequisites</span></span>
<span data-ttu-id="eddfe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eddfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eddfe-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eddfe-109">Permission type</span></span>|<span data-ttu-id="eddfe-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="eddfe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eddfe-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eddfe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eddfe-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eddfe-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="eddfe-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eddfe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eddfe-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eddfe-114">Not supported.</span></span>|
|<span data-ttu-id="eddfe-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eddfe-115">Application</span></span>|<span data-ttu-id="eddfe-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eddfe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eddfe-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eddfe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}
DELETE /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="eddfe-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eddfe-118">Request headers</span></span>
|<span data-ttu-id="eddfe-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eddfe-119">Header</span></span>|<span data-ttu-id="eddfe-120">値</span><span class="sxs-lookup"><span data-stu-id="eddfe-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eddfe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eddfe-121">Authorization</span></span>|<span data-ttu-id="eddfe-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="eddfe-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eddfe-123">承諾</span><span class="sxs-lookup"><span data-stu-id="eddfe-123">Accept</span></span>|<span data-ttu-id="eddfe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eddfe-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eddfe-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="eddfe-125">Request body</span></span>
<span data-ttu-id="eddfe-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="eddfe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eddfe-127">応答</span><span class="sxs-lookup"><span data-stu-id="eddfe-127">Response</span></span>
<span data-ttu-id="eddfe-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="eddfe-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eddfe-129">例</span><span class="sxs-lookup"><span data-stu-id="eddfe-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="eddfe-130">要求</span><span class="sxs-lookup"><span data-stu-id="eddfe-130">Request</span></span>
<span data-ttu-id="eddfe-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eddfe-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="eddfe-132">応答</span><span class="sxs-lookup"><span data-stu-id="eddfe-132">Response</span></span>
<span data-ttu-id="eddfe-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eddfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



