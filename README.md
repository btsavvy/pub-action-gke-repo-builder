# pub-action-gke-repo-builder
pub-action-gke-repo-builder
inputs:
  token:
    description: 'The oauth token'
    required: true
outputs:
  data:
    description: 'The placeholder for any output data'
Repo Config
{
  "$schema": "http://json-schema.org/draft-04/schema#",
  "type": "object",
  "properties": {
    "domains": {
      "type": "array",
      "items": [
        {
          "type": "string"
        },
        {
          "type": "string"
        },
        {
          "type": "string"
        },
        {
          "type": "string"
        },
        {
          "type": "string"
        },
        {
          "type": "string"
        },
        {
          "type": "string"
        }
      ]
    },
    "templates": {
      "type": "array",
      "items": [
        {
          "type": "object",
          "properties": {
            "template_name": {
              "type": "string"
            },
            "repo_org": {
              "type": "string"
            },
            "repo_owner": {
              "type": "string"
            },
            "domain": {
              "type": "string"
            },
            "temp_repo_permission": {
              "type": "array",
              "items": [
                {
                  "type": "object",
                  "properties": {
                    "team_slug": {
                      "type": "string"
                    },
                    "permission": {
                      "type": "string"
                    }
                  },
                  "required": [
                    "team_slug",
                    "permission"
                  ]
                }
              ]
            },
            "workflows": {
              "type": "object",
              "properties": {
                "workflow-template": {
                  "type": "string"
                },
                "flows": {
                  "type": "array",
                  "items": [
                    {
                      "type": "object",
                      "properties": {
                        "flow-name": {
                          "type": "string"
                        },
                        "steps": {
                          "type": "array",
                          "items": [
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "build-trigger": {
                                  "type": "string"
                                },
                                "branch": {
                                  "type": "string"
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "build-trigger",
                                "branch"
                              ]
                            },
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "needs": {
                                  "type": "string"
                                },
                                "deploy-env": {
                                  "type": "array",
                                  "items": [
                                    {
                                      "type": "string"
                                    }
                                  ]
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "needs",
                                "deploy-env"
                              ]
                            }
                          ]
                        }
                      },
                      "required": [
                        "flow-name",
                        "steps"
                      ]
                    },
                    {
                      "type": "object",
                      "properties": {
                        "flow-name": {
                          "type": "string"
                        },
                        "steps": {
                          "type": "array",
                          "items": [
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "build-trigger": {
                                  "type": "string"
                                },
                                "branch": {
                                  "type": "string"
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "build-trigger",
                                "branch"
                              ]
                            },
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "needs": {
                                  "type": "string"
                                },
                                "deploy-env": {
                                  "type": "array",
                                  "items": [
                                    {
                                      "type": "string"
                                    }
                                  ]
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "needs",
                                "deploy-env"
                              ]
                            },
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "needs": {
                                  "type": "string"
                                },
                                "deploy-env": {
                                  "type": "array",
                                  "items": [
                                    {
                                      "type": "string"
                                    }
                                  ]
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "needs",
                                "deploy-env"
                              ]
                            },
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "needs": {
                                  "type": "string"
                                },
                                "deploy-env": {
                                  "type": "array",
                                  "items": [
                                    {
                                      "type": "string"
                                    }
                                  ]
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "needs",
                                "deploy-env"
                              ]
                            },
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "needs": {
                                  "type": "string"
                                },
                                "deploy-env": {
                                  "type": "array",
                                  "items": [
                                    {
                                      "type": "string"
                                    }
                                  ]
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "needs",
                                "deploy-env"
                              ]
                            },
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "needs": {
                                  "type": "string"
                                },
                                "deploy-env": {
                                  "type": "array",
                                  "items": [
                                    {
                                      "type": "string"
                                    }
                                  ]
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "needs",
                                "deploy-env"
                              ]
                            }
                          ]
                        }
                      },
                      "required": [
                        "flow-name",
                        "steps"
                      ]
                    },
                    {
                      "type": "object",
                      "properties": {
                        "flow-name": {
                          "type": "string"
                        },
                        "steps": {
                          "type": "array",
                          "items": [
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "build-trigger": {
                                  "type": "string"
                                },
                                "branch": {
                                  "type": "string"
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "build-trigger",
                                "branch"
                              ]
                            },
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "needs": {
                                  "type": "string"
                                },
                                "deploy-env": {
                                  "type": "array",
                                  "items": [
                                    {
                                      "type": "string"
                                    }
                                  ]
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "needs",
                                "deploy-env"
                              ]
                            },
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "needs": {
                                  "type": "string"
                                },
                                "deploy-env": {
                                  "type": "array",
                                  "items": [
                                    {
                                      "type": "string"
                                    }
                                  ]
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "needs",
                                "deploy-env"
                              ]
                            },
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "needs": {
                                  "type": "string"
                                },
                                "deploy-env": {
                                  "type": "array",
                                  "items": [
                                    {
                                      "type": "string"
                                    }
                                  ]
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "needs",
                                "deploy-env"
                              ]
                            }
                          ]
                        }
                      },
                      "required": [
                        "flow-name",
                        "steps"
                      ]
                    },
                    {
                      "type": "object",
                      "properties": {
                        "flow-name": {
                          "type": "string"
                        },
                        "steps": {
                          "type": "array",
                          "items": [
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "build-trigger": {
                                  "type": "string"
                                },
                                "branch": {
                                  "type": "string"
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "build-trigger",
                                "branch"
                              ]
                            },
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "needs": {
                                  "type": "string"
                                },
                                "deploy-env": {
                                  "type": "array",
                                  "items": [
                                    {
                                      "type": "string"
                                    }
                                  ]
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "needs",
                                "deploy-env"
                              ]
                            },
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "needs": {
                                  "type": "string"
                                },
                                "deploy-env": {
                                  "type": "array",
                                  "items": [
                                    {
                                      "type": "string"
                                    }
                                  ]
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "needs",
                                "deploy-env"
                              ]
                            },
                            {
                              "type": "object",
                              "properties": {
                                "type": {
                                  "type": "string"
                                },
                                "name": {
                                  "type": "string"
                                },
                                "needs": {
                                  "type": "string"
                                },
                                "deploy-env": {
                                  "type": "array",
                                  "items": [
                                    {
                                      "type": "string"
                                    }
                                  ]
                                }
                              },
                              "required": [
                                "type",
                                "name",
                                "needs",
                                "deploy-env"
                              ]
                            }
                          ]
                        }
                      },
                      "required": [
                        "flow-name",
                        "steps"
                      ]
                    }
                  ]
                }
              },
              "required": [
                "workflow-template",
                "flows"
              ]
            },
            "environments": {
              "type": "array",
              "items": [
                {
                  "type": "object",
                  "properties": {
                    "name": {
                      "type": "string"
                    },
                    "reviewers": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        }
                      ]
                    },
                    "prevent-self-review": {
                      "type": "boolean"
                    },
                    "bypass-protection-rules": {
                      "type": "boolean"
                    },
                    "env_var": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        }
                      ]
                    }
                  },
                  "required": [
                    "name",
                    "reviewers",
                    "prevent-self-review",
                    "bypass-protection-rules",
                    "env_var"
                  ]
                },
                {
                  "type": "object",
                  "properties": {
                    "name": {
                      "type": "string"
                    },
                    "reviewers": {
                      "type": "array",
                      "items": {}
                    },
                    "prevent-self-review": {
                      "type": "boolean"
                    },
                    "bypass-protection-rules": {
                      "type": "boolean"
                    },
                    "env_var": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        }
                      ]
                    }
                  },
                  "required": [
                    "name",
                    "reviewers",
                    "prevent-self-review",
                    "bypass-protection-rules",
                    "env_var"
                  ]
                },
                {
                  "type": "object",
                  "properties": {
                    "name": {
                      "type": "string"
                    },
                    "reviewers": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        }
                      ]
                    },
                    "prevent-self-review": {
                      "type": "boolean"
                    },
                    "bypass-protection-rules": {
                      "type": "boolean"
                    },
                    "env_var": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        }
                      ]
                    }
                  },
                  "required": [
                    "name",
                    "reviewers",
                    "prevent-self-review",
                    "bypass-protection-rules",
                    "env_var"
                  ]
                },
                {
                  "type": "object",
                  "properties": {
                    "name": {
                      "type": "string"
                    },
                    "reviewers": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        }
                      ]
                    },
                    "prevent-self-review": {
                      "type": "boolean"
                    },
                    "bypass-protection-rules": {
                      "type": "boolean"
                    },
                    "env_var": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        }
                      ]
                    }
                  },
                  "required": [
                    "name",
                    "reviewers",
                    "prevent-self-review",
                    "bypass-protection-rules",
                    "env_var"
                  ]
                },
                {
                  "type": "object",
                  "properties": {
                    "name": {
                      "type": "string"
                    },
                    "reviewers": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        }
                      ]
                    },
                    "prevent-self-review": {
                      "type": "boolean"
                    },
                    "bypass-protection-rules": {
                      "type": "boolean"
                    },
                    "env_var": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        }
                      ]
                    }
                  },
                  "required": [
                    "name",
                    "reviewers",
                    "prevent-self-review",
                    "bypass-protection-rules",
                    "env_var"
                  ]
                },
                {
                  "type": "object",
                  "properties": {
                    "name": {
                      "type": "string"
                    },
                    "reviewers": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        }
                      ]
                    },
                    "prevent-self-review": {
                      "type": "boolean"
                    },
                    "bypass-protection-rules": {
                      "type": "boolean"
                    },
                    "env_var": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        }
                      ]
                    }
                  },
                  "required": [
                    "name",
                    "reviewers",
                    "prevent-self-review",
                    "bypass-protection-rules",
                    "env_var"
                  ]
                },
                {
                  "type": "object",
                  "properties": {
                    "name": {
                      "type": "string"
                    },
                    "reviewers": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        }
                      ]
                    },
                    "prevent-self-review": {
                      "type": "boolean"
                    },
                    "bypass-protection-rules": {
                      "type": "boolean"
                    },
                    "env_var": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        }
                      ]
                    }
                  },
                  "required": [
                    "name",
                    "reviewers",
                    "prevent-self-review",
                    "bypass-protection-rules",
                    "env_var"
                  ]
                },
                {
                  "type": "object",
                  "properties": {
                    "name": {
                      "type": "string"
                    },
                    "reviewers": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        }
                      ]
                    },
                    "prevent-self-review": {
                      "type": "boolean"
                    },
                    "bypass-protection-rules": {
                      "type": "boolean"
                    },
                    "env_var": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        }
                      ]
                    }
                  },
                  "required": [
                    "name",
                    "reviewers",
                    "prevent-self-review",
                    "bypass-protection-rules",
                    "env_var"
                  ]
                },
                {
                  "type": "object",
                  "properties": {
                    "name": {
                      "type": "string"
                    },
                    "reviewers": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        }
                      ]
                    },
                    "prevent-self-review": {
                      "type": "boolean"
                    },
                    "bypass-protection-rules": {
                      "type": "boolean"
                    },
                    "env_var": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        }
                      ]
                    }
                  },
                  "required": [
                    "name",
                    "reviewers",
                    "prevent-self-review",
                    "bypass-protection-rules",
                    "env_var"
                  ]
                },
                {
                  "type": "object",
                  "properties": {
                    "name": {
                      "type": "string"
                    },
                    "reviewers": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "type": {
                              "type": "string"
                            },
                            "name": {
                              "type": "string"
                            }
                          },
                          "required": [
                            "type",
                            "name"
                          ]
                        }
                      ]
                    },
                    "prevent-self-review": {
                      "type": "boolean"
                    },
                    "bypass-protection-rules": {
                      "type": "boolean"
                    },
                    "env_var": {
                      "type": "array",
                      "items": [
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        },
                        {
                          "type": "object",
                          "properties": {
                            "name": {
                              "type": "string"
                            },
                            "value": {
                              "type": "string"
                            },
                            "lock": {
                              "type": "boolean"
                            }
                          },
                          "required": [
                            "name",
                            "value",
                            "lock"
                          ]
                        }
                      ]
                    }
                  },
                  "required": [
                    "name",
                    "reviewers",
                    "prevent-self-review",
                    "bypass-protection-rules",
                    "env_var"
                  ]
                }
              ]
            }
          },
          "required": [
            "template_name",
            "repo_org",
            "repo_owner",
            "domain",
            "temp_repo_permission",
            "workflows",
            "environments"
          ]
        }
      ]
    }
  },
  "required": [
    "domains",
    "templates"
  ]
}
