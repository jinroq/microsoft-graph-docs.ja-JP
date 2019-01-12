---
title: educationIdentitySynchronizationConfiguration リソースの種類
description: すべて学校データ プロファイルの id の同期設定の抽象基本クラスです。 派生クラスは、識別情報を同期するための動作を定義します。 派生型を次に示します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6d9841d4957d5330fc966f60a24582e101831b6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969031"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>educationIdentitySynchronizationConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

すべて学校データ プロファイルの id の同期設定の抽象基本クラスです。 派生クラスは、識別情報を同期するための動作を定義します。 派生型を次に示します。

## <a name="derived-types"></a>派生型
| Type | 説明 | 
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | Azure Active Directory (AD の Azure) 内の既存のユーザー アカウントを一致させるには、この型を使用します。 |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | Azure AD で新しいユーザー アカウントを作成するのにには、この型を使用します。 |
